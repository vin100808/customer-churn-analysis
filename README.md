# Customer Churn Prediction

A machine learning project to predict customer churn and identify key drivers using structured data. The project focuses on actionable insights to support customer retention strategies.

## 📌 Objective

- Predict which customers are likely to churn based on service and demographic features
- Identify the most important factors contributing to churn
- Provide data-driven business recommendations

## 📂 Data

- Dataset: [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- 7043 rows, 21 features including contract type, internet service, and monthly charges

## 🛠️ Tools Used

- Python (pandas, numpy, seaborn, matplotlib)
- Machine Learning: Random Forest, XGBoost
- Model Evaluation: Accuracy, Precision, Recall, F1-score
- Feature Importance Analysis

## 📊 Key Findings

- Customers with **fiber optic internet service** have a **churn rate of 41.9%**, compared to 14.5% for others
- Customers with **two-year contracts** have a churn rate of only **2.8%**, compared to 34.1% for others
- These two features were consistently ranked as the most important in both Random Forest and XGBoost models

## ✅ Business Insights

- Fiber optic users are high-risk customers. Consider addressing pricing, service quality, or expectations.
- Long-term contracts significantly reduce churn. Bundling them with fiber plans could be a high-impact strategy.

## 📈 Model Performance (XGBoost)

- Accuracy: 80%
- Recall (churned customers): 52%
- F1-score: 59%

## 📁 File Structure

<pre><code>```bash customer-churn-analysis/ ├── data/ │ ├── WA_Fn-UseC_-Telco-Customer-Churn.csv │ ├── cleaned_data.csv │ └── cleaned_data.pkl │ ├── notebooks/ │ ├── 01_data_cleaning.ipynb │ ├── 02_eda_visualization.ipynb │ ├── 03_modeling.ipynb │ └── output/ │ ├── classification_report_xgb.txt │ ├── classification_report_rf.txt │ ├── feature_importance_xgb.png │ └── feature_importance_rf.png │ ├── dashboard/ │ └── churn_dashboard.twbx │ ├── requirements.txt ├── README.md └── .gitignore ```</code></pre>

```bash

customer-churn-prediction/
│
├── data/                       
│   ├── WA_Fn-UseC_-Telco-Customer-Churn.csv
│   ├── cleaned_data.pkl
│   └── cleaned_data.csv
│
├── notebooks/                    
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda_visualization.ipynb
│   └── 03_modeling.ipynb
│
├── output/                       
│   ├── feature_importance_rf.png
│   ├── feature_importance_xgb.png
│   ├── classification_report_rf.txt
│   └── classification_report_xgb.txt
│
├── dashboard/                    
│   └── churn_dashboard.twbx
│
├── requirements.txt              
├── README.md                     
└── .gitignore                    

```

## 🔖 Author

Zhiming Lin  
Master of Management Analytics – Queen’s University