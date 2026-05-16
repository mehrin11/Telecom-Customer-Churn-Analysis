[README.md](https://github.com/user-attachments/files/27853667/README.md)
📊 Telecom Customer Churn Analysis
A data analysis project exploring why customers leave a telecom company, using the Telco Customer Churn dataset from Kaggle.
## 🔍 Problem
Why do customers leave a telecom company? Can we find patterns that help the business retain them?
## 📁 Dataset
- **Source:** [Kaggle – Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Size:** 7,043 customers, 21 features
- **Key columns:** `tenure`, `Contract`, `MonthlyCharges`, `TotalCharges`, `Churn`
## 🗂️ Project Structure
telco-churn-analysis/
├── data/                  ← Place the CSV file here
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── notebooks/
│   └── churn_analysis.ipynb   ← Main analysis notebook
├── charts/                ← Auto-generated charts
│   ├── churn_by_contract.png          ← % churn by contract type
│   ├── monthly_charges_vs_churn.png   ← boxplot of charges vs churn
│   ├── tenure_vs_churn.png            ← churn proportion by tenure band
│   └── churn_by_internet_service.png  ← % churn by internet service type
└── README.md
## ⚙️ Setup & How to Run
### Requirements
- Python 3.8+ (via [Anaconda](https://anaconda.com))
- Libraries: `pandas`, `matplotlib`, `seaborn` (all included with Anaconda)
### Steps
1. Download the dataset from Kaggle and place it in the `data/` folder
2. Open Anaconda Navigator → launch Jupyter Notebook
3. Navigate to `notebooks/churn_analysis.ipynb`
4. Run all cells top to bottom (`Kernel → Restart & Run All`)
## 📊 Key Findings

| # | Finding | Detail |
|---|---------|--------|
| 1 | **Month-to-month customers churn at 42.7%** | vs 11.3% for one-year and just 2.8% for two-year contracts — a 15x gap |
| 2 | **Churned customers pay ~$14 more per month** | Median $79/mo vs $65/mo for retained customers |
| 3 | **~57% of month-1 customers churn** | Churn drops sharply after month 12 and stabilises below 15% after month 24 |
| 4 | **Fiber optic customers churn at 41.9%** | More than double DSL (19%) — a product-level retention problem |

## 💡 Business Recommendations

1. **Convert month-to-month customers to annual contracts early** — especially in the first 3 months; the churn gap vs two-year contracts is 15x
2. **Prioritise first-year onboarding** — churn is highest at month 1 (~57%) and drops sharply after month 12
3. **Investigate fiber optic pricing and service quality** — at 41.9% churn it is as problematic as month-to-month contracts
4. **Target high-paying new customers with retention offers** — churned customers pay $14 more per month, signalling price dissatisfaction

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| Python (pandas) | Data loading, cleaning, and analysis |
| Matplotlib / Seaborn | Data visualization |
| Jupyter Notebook | Interactive coding environment |
| Tableau Public | Final interactive dashboard |

## 📈 Dashboard

> 🔗 **[View Live Dashboard on Tableau Public](https://public.tableau.com/views/P3_17789301874540/Dashboard1?:language=en-GB&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)**
