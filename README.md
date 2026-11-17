# 🎬 Netflix Customer Churn Prediction System

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Machine%20Learning-Classification-orange" />
  <img src="https://img.shields.io/badge/Scikit--Learn-Modeling-F7931E?logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/Status-Completed-success" />
</p>

<p align="center">
  <b>An End-to-End Machine Learning Project for Predicting Customer Churn</b>
</p>

---

## 📌 Project Overview

Customer churn is a major challenge for subscription-based businesses. Retaining existing customers is essential for long-term growth and customer satisfaction.

This project develops a **Machine Learning-based Customer Churn Prediction System** using a synthetic Netflix-style dataset containing 10,000 customer records.

The system analyses customer demographics, subscription information, viewing behaviour, satisfaction levels, and payment history to identify customers who are likely to discontinue their subscriptions.

## 🎯 Project Objectives

- Identify patterns and factors associated with customer churn.
- Perform data cleaning and exploratory data analysis.
- Engineer meaningful features to improve predictive modelling.
- Train and compare multiple Machine Learning algorithms.
- Evaluate and optimize model performance.
- Predict churn probabilities for individual and multiple customers.

## 📂 Dataset Information

| Attribute | Description |
|---|---|
| Dataset size | 10,000 original customer records |
| Data type | Synthetic customer data |
| Features | Customer demographics, subscription and behaviour |
| Target variable | Churn Status (Yes/No) |
| Problem type | Binary Classification |

**Major dataset attributes:**
- Customer satisfaction and engagement rate
- Daily watch time
- Subscription length and plan
- Payment history
- Device and genre preferences
- Age and monthly income
- Support queries and promotional offers

## ⚙️ Project Workflow

1. **Data Collection:** Generated a synthetic Netflix-style customer dataset.
2. **Data Cleaning:** Handled missing values, duplicate records, invalid values, and inconsistent categorical labels.
3. **Exploratory Data Analysis:** Analysed churn distribution, customer behaviour, and feature relationships using visualizations.
4. **Feature Engineering:** Created behavioural indicators such as Low Watch Time, Low Engagement, Payment Risk, and other customer-related features.
5. **Model Training:** Implemented three classification algorithms.
6. **Model Evaluation:** Compared model performance using multiple evaluation metrics.
7. **Model Optimization:** Applied cross-validation and classification threshold tuning.
8. **Churn Prediction:** Generated individual customer predictions and churn probabilities.

## 🤖 Machine Learning Models

The following algorithms were implemented and compared:

- Logistic Regression
- Random Forest Classifier
- Gradient Boosting Classifier

## 📊 Model Performance

Test-set performance comparison:

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 64.46% | 38.07% | **67.81%** | **48.76%** | **0.7303** |
| Random Forest | 76.17% | 60.38% | 12.96% | 21.33% | 0.7033 |
| Gradient Boosting | **77.03%** | **62.58%** | 19.64% | 29.89% | 0.7171 |

### 🏆 Selected Model: Logistic Regression

Logistic Regression was selected as the leading candidate because it achieved:

- Highest test ROC-AUC: **0.7303**
- Highest churn recall: **67.81%**
- Highest F1-score: **48.76%**
- Highest 5-fold cross-validation ROC-AUC: **0.7332**

Although Gradient Boosting achieved higher accuracy, Logistic Regression identified a greater proportion of actual churners, making it more suitable for the project's churn identification objective.

*Note: The metrics above are from the default-threshold model comparison. The final tuned-threshold evaluation should be reported separately.*

## 📈 Model Evaluation Techniques

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix
- ROC Curve
- 5-Fold Cross-Validation
- Classification Threshold Optimization

## 🔍 Customer Churn Prediction

The final prediction notebook uses the selected Logistic Regression pipeline to:

- Predict whether an individual customer is likely to churn.
- Calculate churn and retention probabilities.
- Apply a selected classification threshold.
- Test multiple customer profiles.
- Display structured customer prediction results.

## 🛠️ Technologies Used

| Category | Tools |
|---|---|
| Programming Language | Python |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Development Environment | Google Colab, Jupyter Notebook |
| Model Saving | Joblib |

## 📁 Repository Structure

```text
Netflix-Customer-Churn-Prediction/
│
├── data/
│   ├── raw_data.csv
│   ├── cleaned_data.csv
│   └── features_engineered_data.csv
│
├── notebooks/
│   ├── Data_Cleaning.ipynb
│   ├── Netflix_EDA.ipynb
│   ├── Feature_Engineering.ipynb
│   ├── training.ipynb
│   └── churn_prediction.ipynb
│
├── models/
│   └── netflix_churn_final_model.pkl
│
├── README.md
└── .gitignore
```

## 🚀 How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/Netflix-Customer-Churn-Prediction.git
```

2. Navigate to the project directory:

```bash
cd Netflix-Customer-Churn-Prediction
```

3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib
```

4. Open the notebooks using Jupyter Notebook or Google Colab.

5. Run the notebooks in the following order:

   - Data Cleaning
   - Exploratory Data Analysis
   - Feature Engineering
   - Model Training
   - Churn Prediction

6. Ensure the dataset and saved model paths are configured correctly.

## 💡 Key Learnings

- Practical experience with end-to-end Machine Learning workflows.
- Handling missing values, duplicate records, and inconsistent data.
- Understanding customer behaviour through EDA.
- Feature engineering and preprocessing using Scikit-learn.
- Comparing classification algorithms.
- Evaluating models using cross-validation and multiple metrics.
- Understanding the precision-recall trade-off and threshold optimization.





---

⭐ If you find this project interesting, consider giving the repository a star!
