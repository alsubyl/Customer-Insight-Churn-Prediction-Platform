# Project in progress - modeling and deployment ongoing
# Customer-Insight-Churn-Prediction-Platform

An end-to-end data analytics project focused on analyzing customer behavior and predicting customer churn using machine learning.  
The project aims to support data-driven business decisions through structured data preprocessing, predictive modeling, SQL analysis, interactive dashboards, and a Streamlit-based web application.



## Project Overview

Customer churn is a critical challenge for many subscription-based businesses.  
This project provides a comprehensive analytical pipeline to explore customer data, identify churn patterns, and build predictive models that help organizations proactively retain customers.

The platform follows a structured workflow that includes:
- Data exploration and preprocessing
- Feature engineering and encoding
- Machine learning model development (planned)
- Analytical insights using SQL
- Business dashboards and visualizations
- A deployable web application for predictions (planned)



## Dataset

This project uses the **Telco Customer Churn** dataset.

The raw dataset is included in this repository for reproducibility and ease of use:
data/raw_dataset.csv

The dataset was originally sourced from Kaggle:
- Telco Customer Churn Dataset

It contains customer-level information such as:
- Demographics (e.g., gender, senior citizen)
- Subscription details (e.g., contract type, internet service)
- Billing and payment information
- Churn status (target variable)

### Reproducibility

To reproduce the preprocessing steps:
1. Use the provided raw dataset located in the `data/` directory
2. Run the data preprocessing notebook to generate the processed datasets

Processed datasets are generated programmatically during preprocessing and modeling stages and are intentionally not committed to the repository to maintain flexibility and avoid redundancy.



## Preprocessing

The preprocessing stage focuses on cleaning the data, handling data types, encoding categorical variables, and preparing the dataset for machine learning workflows.

Key steps include:
- Data type correction and validation
- One-Hot Encoding of categorical features
- Train–test splitting with stratification
- Clear separation between model-independent preprocessing and modeling-specific steps

> **Note on Encoding Strategy and Data Leakage**  
> For simplicity, One-Hot Encoding was applied before the train–test split in the preprocessing notebook.  
> In the final modeling stage, a `Pipeline` with `OneHotEncoder(handle_unknown="ignore")` will be used to avoid data leakage and safely handle unseen categories.



## Modeling *(Planned)*

This section will include:
- Model selection and comparison
- Feature scaling where required
- Handling class imbalance
- Evaluation metrics and performance analysis



## Dashboards & Application *(Planned)*

- SQL-based analytical queries
- Interactive dashboards (Power BI)
- A Streamlit web application for churn prediction



## Repository Structure
Customer-Insight-Churn-Prediction-Platform/

├── app/                 # Streamlit application (planned)

├── dashboard/           # Dashboard files

├── data/

│   ├── raw_dataset.csv  # Raw Telco Customer Churn dataset

│   └── processed/       # Generated locally (not committed)

├── model/               # Saved models (planned)

├── notebooks/           # Jupyter notebooks (EDA & preprocessing)

├── sql/                 # SQL analysis

└── README.md





## Author

This project is part of a data analytics and machine learning portfolio and is under active development.



