# 🛡️ Insurance-Claim-Prediction-System

## 📌 Project Overview

This project focuses on building a machine learning model to predict the risk of an insurance claim occurring within the next 6 months. The objective is to help insurance companies assess customer risk more accurately and support better premium pricing decisions.
___________________________________________________________________________________________________

## 📁 Project Structure

<pre>
insurance-claim-risk-prediction/
│
├── notebooks/
│   └── insurance_claim_model.ipynb
│
├── presentation/
│   └── car_insurance_claim_prediction_presentation.pptx
│
├── data/
│   └── (sample raw data)
│
├── README.md
│
└── requirements.txt
</pre>
___________________________________________________________________________________________________


## ⚠️ Key Challenges
While working on this project, I faced several real-world data challenges:
- Imbalanced Dataset:
The target variable is_claim had only around 6% positive cases, which caused strong class imbalance.
- High Cardinality Feature:
One categorical column had a very large number of unique values, making it difficult to encode effectively.
- Irrelevant Features:
The dataset contained many car-specific columns that did not add much predictive value.
___________________________________________________________________________________________________


## 🛠️ Solutions Implemented

- To handle class imbalance, I applied the SMOTE-Tomek technique to balance the target variable by creating synthetic minority samples and cleaning overlapping data points.
- To solve the high cardinality issue, I used Target Encoding, ensuring it was applied only on training data to avoid data leakage.
- For irrelevant features, I performed feature engineering by creating new derived features and removing less useful ones.
___________________________________________________________________________________________________


## 🤖 Modeling Approach
I trained multiple models, including Random Forest and XGBoost, and experimented with:

- Training with and without SMOTE-Tomek
- Different feature combinations
- Model parameter variations
___________________________________________________________________________________________________


## 📊 Results & Learnings

Despite trying multiple approaches, the model did not achieve strong accuracy or F1 scores. This analysis revealed that the primary limitation lies in the dataset itself, which lacks sufficient informative features rather than the modeling techniques used.

This project helped me understand the importance of data quality, feature relevance, and realistic expectations when working with real-world datasets.
