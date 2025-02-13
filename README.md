# Financial Advisor Matching Model - NUS Datathon Project

# Overview

This project was developed as part of the NUS Datathon 2024, where the objective was to build a machine learning model to recommend the most suitable financial advisors to customers. By leveraging data science techniques, the goal is to enhance engagement, improve policy conversion rates, and drive revenue growth for financial services.

# Dataset

The dataset provided consisted of anonymized customer, agent, and policy data:

Customer Table: Demographics such as gender, marital status, economic status, and household size.

Agent Table: Financial advisor details, including tenure, expertise, and past performance.

Policy Table: Information on policies, customer-agent relationships, and policy statuses.

# Methodology

1. Data Preprocessing

Handling Missing Values: Used imputation techniques such as mean/mode replacement and KNN imputation.

Feature Engineering:

Created derived features, such as agent-to-customer interaction ratios and policy conversion rates.

Encoded categorical variables using one-hot encoding and target encoding.

Standardized numerical variables using StandardScaler to ensure comparability.

Data Splitting: 80% training data, 20% testing data.

2. Model Selection & Training

Several machine learning approaches were explored:

Collaborative Filtering: Used SVD and KNN-based models.

Supervised Learning: Tested models including Logistic Regression, Random Forest, XGBoost, and Neural Networks.

Unsupervised Learning: Applied clustering techniques (K-Means, Hierarchical Clustering) for customer and advisor segmentation.

Hyperparameter tuning was performed using Grid Search and Bayesian Optimization.

3. Model Evaluation

The following metrics were used to assess performance:

Precision@k, Recall@k: Measures accuracy of the top-k recommended advisors.

NDCG@k: Evaluates ranking effectiveness.

F1-Score: Balances precision and recall.

AUC-ROC Curve: Assesses classification performance.

# Results & Insights

Business Impact

Improved conversion rates due to better customer-advisor matching.

Increased customer engagement and policy retention.

Ensured fairness in recommendations to promote diversity among advisors.

# Future Enhancements

Incorporate external socioeconomic data for better predictions.

Implement deep learning architectures for improved personalization.

Develop real-time recommendation systems for dynamic customer interactions.

# Project Setup

1. Prerequisites

Ensure you have the necessary Python packages installed:

pip install -r requirements.txt

2. Running the Model

Execute the following command to run the Jupyter notebook:

jupyter notebook CAT_A_<TEAM_NUMBER>.ipynb

Ensure that the dataset is correctly loaded into the notebook.

3. Reproducing Results

Follow these steps:

Load the dataset (ensure correct file paths are provided in the notebook).

Preprocess the data using the methods described in the notebook.

Train the model using the pre-configured pipeline.

Evaluate the model using the defined metrics.

4. Submission Details

Submission Folder Name: NUS_DATATHON_CAT_A_63

Files included:

CAT_A_63.ipynb: Jupyter notebook with full implementation.

requirements.txt: List of necessary Python packages.

model.pkl (if applicable): Saved model file.

README.pdf: Setup instructions and methodology.

Report.pdf: Detailed analysis and results.

For any issues, refer to the comments in the notebook or reach out to the organizers.

This repository contains all necessary code and documentation to replicate the financial advisor recommendation system developed for the NUS Datathon 2024.

