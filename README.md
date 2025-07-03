# Anti-Money-Laundering-AML-Risk-Detection-and-Fraud-Analysis


This project focuses on detecting high-risk transactions and potential fraud patterns using transactional behavior data. It combines Python-based feature engineering and Power BI visual analytics to uncover hidden risk insights.

---

## 📌 Objective
- Detect and analyze suspicious transaction behaviors.
- Identify ghost accounts, drained accounts, and transaction type patterns.
- Visualize KPIs and risk trends using Power BI.


---

## 🔧 Tools Used
- Python (Pandas, Matplotlib, Seaborn)
- Power BI (KPIs, DAX, Charts)
- Jupyter Notebook
- Git & GitHub

---

## 📂 Files in This Repo

| File | Description |
|------|-------------|
| `Jupyter_Analysis.ipynb` | Data cleaning, fraud logic, and high-risk tagging |
| `AML_Risk_Dashboard.pbix` | Fully interactive Power BI dashboard |
| `README.md` | Project overview |
| `images/` | Dashboard & chart screenshots |
| `data/` | Optional: Cleaned transaction CSV |

---

## 📈 Key Insights

- **8213 High-Risk Transactions** detected
- **~50% Ghost Transactions** indicate account anomalies
- **Transfer & Cash-Out** dominate high-risk types
- **Transaction spikes** at specific steps may indicate coordinated fraud
- Only **15 origin accounts** had drained balances (red flag)

---

## 🔍 Risk Detection Logic

- **Ghost Accounts**: `oldbalanceDest == 0` and `newbalanceDest == 0` but `amount > 0`
- **Drained Accounts**: `oldbalanceOrig > 0` and `newbalanceOrig == 0`
- **Risk Levels**: Based on pattern flags and `isFraud`/`isFlaggedFraud`

---

## 📘 How to Use

1. Clone this repo
2. Open `Jupyter_Analysis.ipynb` to explore Python logic
3. Open `AML_Risk_Dashboard.pbix` in Power BI Desktop to interact with the dashboard
4. Optional: Upload data to update visuals

---

## 📁 Dataset Source

- Original dataset from Kaggle: [PaySim – Fraud Detection](https://www.kaggle.com/datasets/ntnu-testimon/paysim1)
- Due to licensing and size constraints, raw data is not included in this repository.
- Only the filtered **high-risk transactions** (`high_risk_transactions.csv`) are used and shared for dashboard visualization.

The original data was sourced from the Kaggle PaySim Dataset (Synthetic Financial Dataset for Fraud Detection). Due to size/licensing, raw data is not uploaded here. Only transformed outputs are shared

## 📬 Contact

If you found this useful or want to collaborate, feel free to connect:

Amal s  
📧 amal17ek@gmail.com  
🔗 linkedin.com/in/amal-s-9a5b86310
