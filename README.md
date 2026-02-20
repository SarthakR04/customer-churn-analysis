# 🚀 End-to-End Customer Churn Analysis & Prediction

## 📊 Project Overview

This project demonstrates a complete end-to-end Customer Churn Analysis
pipeline for a Telecom company using SQL, Power BI, and Machine
Learning.

The goal was to:

-   Analyze historical customer churn behavior
-   Identify key churn drivers
-   Build a predictive model for future churners
-   Visualize high-risk customers to support retention strategies

------------------------------------------------------------------------

## 🛠 Tech Stack

-   **SQL Server** -- ETL & Data Preparation
-   **Power BI** -- Dashboard Development & KPI Analysis
-   **Python (Jupyter Notebook)** -- Machine Learning
-   **Pandas & NumPy** -- Data Processing
-   **Scikit-learn** -- Random Forest Model
-   **Matplotlib & Seaborn** -- Visualization

------------------------------------------------------------------------

## 🔄 Project Workflow

### 1️⃣ Data Engineering (SQL)

-   Created staging and production tables
-   Cleaned null values and standardized categorical variables
-   Built analytical views for BI consumption:
    -   `vw_ChurnData`
    -   `vw_JoinData`

------------------------------------------------------------------------

### 2️⃣ Business Intelligence (Power BI)

Developed interactive dashboards including:

-   Total Customers
-   Total Churn & Churn Rate
-   New Joiners
-   Demographic Analysis
-   Contract & Payment Method Insights
-   Geographic Distribution
-   Service Usage Impact

------------------------------------------------------------------------

### 3️⃣ Machine Learning (Random Forest)

-   Train/Test Split: **80/20**
-   Model Accuracy: **84%**
-   Evaluation using Confusion Matrix & Classification Report
-   Feature Importance Analysis

#### 🔝 Top Churn Drivers Identified:

-   Contract Type
-   Total Revenue
-   Total Charges
-   Monthly Charge
-   Tenure in Months

------------------------------------------------------------------------

## 🔎 Model Prediction Insight

When applied to newly joined customers, the model predicted a high
proportion of churn-risk customers.

This behavior is primarily driven by tenure-based learning from
historical data, where low tenure strongly correlates with churn.

Since newly joined customers naturally have lower tenure, the model
assigns higher churn probabilities to this segment.

In real-world deployment, threshold tuning and business validation would
be applied to balance false positives and optimize retention strategy
costs.

------------------------------------------------------------------------

### Power BI Dashboard

The interactive Power BI dashboard was developed to analyze churn metrics and high-risk customers.  
Due to file size constraints, the `.pbix` file is not included in this repository.  

Dashboard previews are available in the **images/** folder.

------------------------------------------------------------------------

## 📁 Repository Structure



- notebook/
  - churn_prediction.ipynb
- PowerBI_images/
  - summary_dashboard.png
  - churn_prediction_page.png
- Data/
  - Prediction_data.csv
  - Predictions.csv
- requirements.txt
- README.md

------------------------------------------------------------------------

## 🚀 Future Enhancements

-   ROC-AUC evaluation
-   Threshold tuning
-   Model comparison (Logistic Regression / XGBoost)
-   Deployment using Streamlit or API

