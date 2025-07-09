# 📊 Customer Churn Prediction - Final Report

## 1. Project Objective
The main goal of this project is to predict customer churn for a telecommunications company. Churn prediction helps identify customers likely to leave the service, allowing the company to proactively implement retention strategies, reduce revenue loss, and improve customer satisfaction.

## 2. Data Overview
The dataset consists of customer information including demographic details, service subscription types, tenure, and billing data. Key features include:
- **CustomerID:** Unique identifier for each customer
- **Gender, SeniorCitizen, Partner, Dependents:** Demographic info
- **Tenure:** Number of months the customer has stayed
- **Contract:** Type of service contract (Month-to-month, One year, Two year)
- **MonthlyCharges, TotalCharges:** Billing amounts
- **Churn:** Target variable indicating if a customer has churned (Yes/No)

## 3. Data Cleaning & Preprocessing
- Removed rows with missing values in critical columns (e.g., TotalCharges).
- Converted categorical variables into numeric form via one-hot encoding.
- Balanced the dataset using SMOTE to address class imbalance and improve model performance.

## 4. Exploratory Data Analysis (EDA)
Performed EDA to uncover patterns and insights:
- Visualized churn distribution to understand class imbalance.
- Analyzed churn rate by contract type showing month-to-month contracts have higher churn.
- Examined monthly charges and tenure distributions in relation to churn.
- Used boxplots and histograms for key features to guide feature engineering.

## 5. Model Building
- Selected **Random Forest Classifier** for its robustness and interpretability.
- Split data into training and test sets.
- Tuned hyperparameters using GridSearchCV to optimize model performance.
- Incorporated class weights and oversampling to handle imbalanced data.

## 6. Model Evaluation
Evaluated the model using:
- **Accuracy:** Overall correct prediction rate.
- **Classification report:** Precision, recall, F1-score for both churn and non-churn classes.
- **Confusion matrix:** Detailed counts of true positives, false positives, true negatives, and false negatives.

## 7. Feature Importance
- Extracted and visualized the top 10 most important features contributing to churn prediction.
- Key drivers include contract type, monthly charges, tenure, and customer demographics.

## 8. Conclusion & Recommendations
- Customers on month-to-month contracts with higher monthly charges and shorter tenure are more likely to churn.
- Business should target these high-risk customers with personalized retention campaigns, discounts, or contract incentives.
- Regular monitoring of churn patterns and updating the predictive model will further help reduce customer attrition and improve profitability.
