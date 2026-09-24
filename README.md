# Customer Churn Prediction using Data Analytics and AI

**AICTE | IBM SkillsBuild Data Analytics with AI Internship 2026 | BharatCares**

## Project Description
Telecom companies lose money when customers leave (this is called *churn*). This project studies 7,043 telecom customers, finds the reasons why customers leave, and builds machine learning models that predict which customers are at risk.

The output is:
- Charts that show what drives churn
- A comparison of 3 machine learning models
- A ranked list of high-risk customers
- Simple business recommendations to reduce churn

## Dataset
- **Name:** IBM Telco Customer Churn
- **Source (GitHub):** https://github.com/IBM/telco-customer-churn-on-icp4d
- **Direct CSV link:** https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv
- **Size:** 7,043 rows, 21 columns
- **Target column:** `Churn` (Yes / No)

The notebook loads the data directly from the link above. If you have no internet, download the CSV, save it as `churn.csv` in the same folder as the notebook, and run it again.

## Technologies Used
- Python 3.9+
- pandas, numpy (data handling)
- matplotlib, seaborn (charts)
- scikit-learn (machine learning: Logistic Regression, Random Forest, Gradient Boosting)
- Jupyter Notebook

## Project Files
| File | What it is |
|---|---|
| `Omkar_CustomerChurnPrediction.ipynb` | Full project code with outputs |
| `requirements.txt` | Python libraries needed |
| `Omkar_ProjectReport.docx` | Project report |
| `README.md` | This file |

## How to Run
1. Install Python 3.9 or newer.
2. Open a terminal in the project folder and run:
   ```
   pip install -r requirements.txt
   jupyter notebook
   ```
3. Open `Omkar_CustomerChurnPrediction.ipynb`.
4. Click **Kernel > Restart & Run All**.

Running the notebook creates a `figures/` folder with charts, plus `model_results.csv` and `high_risk_customers.csv`.

## Key Results
- About **26.6%** of customers churn.
- Churn is highest for **month-to-month contracts (42.7%)**, **new customers**, **fiber optic internet (41.9%)** and **electronic check payers (45.3%)**.
- Customers with online security or tech support churn far less (about 15% vs 42%).
- Best model (by F1 score): **Random Forest** with about **79% recall** and **0.84 ROC-AUC**.
- In the test data, the model's High risk group churned at **63%** while the Low risk group churned at only **8%**.

## Limitations
- The data is a single snapshot in time.
- Patterns found are links, not proven causes.
- No cost data is included, so the money value of retention offers is not calculated.
