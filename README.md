# 📉 Customer Churn Analysis

An end-to-end exploratory data analysis project on a telecom customer dataset to uncover the key drivers of customer churn — helping businesses understand *who* is leaving and *why*.

---

## 📌 Problem Statement

Customer churn is one of the most costly challenges for subscription-based businesses. Losing a customer means losing recurring revenue and incurring the cost of acquiring a replacement. This project analyzes a telecom company's customer data to identify the behavioral patterns, service usage habits, and demographic factors most strongly associated with churn.

---

## 📂 Dataset

| Property | Detail |
|---|---|
| Source | [Telco Customer Churn — IBM Sample Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) |
| Rows | 7,043 customers |
| Features | 21 columns |
| Target | `Churn` (Yes / No) |

**Key features include:**

- **Demographics** — gender, SeniorCitizen, Partner, Dependents
- **Account info** — tenure, Contract type, PaperlessBilling, PaymentMethod, MonthlyCharges, TotalCharges
- **Services subscribed** — PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies

---

## 🔍 Key Findings

### Overall Churn Rate
- **26.5%** of customers have churned — a significant portion worth targeted intervention.

### Demographics
- **Gender** has no meaningful impact on churn — male and female customers churn at nearly equal rates.
- **Senior citizens** churn at a disproportionately higher rate compared to non-senior customers, making them a high-risk segment.

### Tenure
- Customers who are **new (low tenure)** are far more likely to churn.
- Long-tenured customers are much more loyal — churn rate drops significantly after the first year.

### Contract Type
- **Month-to-month** contract customers churn the most by a large margin.
- Customers on **1-year or 2-year contracts** are significantly more retained — longer commitments strongly correlate with loyalty.

### Services
- Customers **without** OnlineSecurity, TechSupport, or OnlineBackup are noticeably more likely to churn.
- **Internet Service type** matters — fiber optic customers churn more than DSL customers, possibly due to price sensitivity.
- Customers with **no additional services** bundled are at higher risk.

### Payment Method
- Customers paying via **electronic check** churn the most compared to other payment methods (credit card, bank transfer, mailed check).

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| Pandas | Data loading, cleaning, manipulation |
| NumPy | Numerical operations |
| Matplotlib | Base plotting |
| Seaborn | Statistical visualizations |
| Jupyter Notebook | Interactive analysis environment |

---

## 📁 Project Structure

```
customer-churn-analysis/
├── Customer_Churn_analysis.ipynb   # Main analysis notebook
├── Customer_Churn.csv              # Dataset
└── README.md
```

---

## 🚀 How to Run

**1. Clone the repository**
```bash
git clone https://github.com/your-username/customer-churn-analysis.git
cd customer-churn-analysis
```

**2. Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

**3. Launch the notebook**
```bash
jupyter notebook Customer_Churn_analysis.ipynb
```

---

## 📊 Visualizations Included

- Churn distribution (count plot + pie chart)
- Churn by gender
- Churn by senior citizen status (stacked bar with percentages)
- Tenure distribution by churn (histogram)
- Churn by contract type
- Churn across all 9 service features (subplot grid)
- Churn by payment method

---

## 💡 Business Recommendations

Based on the analysis, the following actions could reduce churn:

1. **Incentivize long-term contracts** — offer discounts or perks for customers switching from month-to-month to annual plans.
2. **Target new customers early** — implement onboarding programs for customers in their first 3–6 months, when churn risk is highest.
3. **Bundle value-added services** — promote OnlineSecurity and TechSupport bundles, especially to customers who haven't adopted them.
4. **Senior citizen retention program** — create dedicated support or pricing plans for the senior segment, which churns at higher rates.
5. **Review electronic check experience** — investigate whether friction in the electronic check payment process is contributing to dissatisfaction.

---

## 🔮 Future Work

- Build a **predictive churn model** (Logistic Regression, Random Forest, XGBoost) to score individual customers by churn probability
- Perform **feature importance analysis** to rank the strongest predictors
- Build a **customer segmentation** layer using clustering (K-Means) to group customers by risk profile
- Create an interactive **dashboard** in Power BI or Streamlit for business stakeholders

---

## 🙋 Author

**Shatabdi Sen Prapti**  
[LinkedIn](https://www.linkedin.com/in/shatabdi-sen-prapti-030680201/) · [GitHub](https://github.com/your-username)
