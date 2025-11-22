# Customer Churn Prediction (Telecom)

**Project:** Predict which customers are likely to leave the telecom provider using machine learning models.

## Overview
This repository contains the analysis, modeling code, and results for the Telco Customer Churn dataset. The primary objective is to build a classification model that identifies customers at risk of churn and provide actionable insights for retention.

## Repo structure
├── notebooks/

|   └── Customer_Churn_Colab.ipynb

├── data/

│ └── sample_telco.csv (small sample or instructions)

├── models/

│ └── churn_xgb_model.pkl (optional)

├── reports/

│ └── Churn_Project_Report.pdf

├── requirements.txt

├── .gitignore

└── README.md

## Dataset
Source: Kaggle — `Telco Customer Churn`  
(Place the CSV file `Telco-Customer-Churn.csv` into `data/` after downloading from Kaggle.)

## How to run
1. Create virtual environment:
```bash
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
pip install -r requirements.txt
```

2. Open the notebook:
run the notebook in Google Colab.

## Key steps performed
* Data cleaning and preprocessing (handle TotalCharges, encoding categoricals)
* Exploratory Data Analysis (EDA) and visualization
* Feature engineering (tenure groups, service count)
* Model training and comparison: Logistic Regression, Random Forest, XGBoost
* Model evaluation using Accuracy, Precision, Recall, F1, ROC-AUC
* Recommendations for business actions and next steps

## Results (summary)
- Best model: XGBoost (ROC-AUC ~0.90+, high recall)
- Business insight: Month-to-month customers and electronic check payers are more likely to churn.

## Notes
+ Large raw dataset is not included. Download from Kaggle and place in data/.
+ For interpretability, consider running SHAP analysis (not included).

## License
-This project is released under the MIT License. See LICENSE for details.

## Contact
Drushti Vagal — drushtivagal22@gmail.com

Project Colab: https://colab.research.google.com/drive/1e7-kB9kc0cag2XJUJ8ghCmg2UVY-oMHX?usp=sharing
