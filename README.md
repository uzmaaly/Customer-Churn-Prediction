# Customer-Churn-Prediction

## Project Overview

This project aims to predict **customer churn** for a bank using a dataset of customer information. Churn refers to the loss of customers, and being able to accurately predict churn allows businesses to implement retention strategies for high-risk customers. This analysis focuses on identifying patterns that distinguish customers who are likely to leave the bank from those who are not.

## Dataset
The dataset consists of features related to customer demographics and behaviour. Key features include:
* Credit Score: A customer’s credit score.
* Geography: The country of the customer.
* Gender: Male or Female.
* Age: Age of the customer.
* Balance: Bank balance of the customer.
* Products: Number of products that the customer uses.
* Debit_Card: Whether the customer owns a credit card.
* Active Member: Whether the customer is an active member of the bank.
* Estimated Salary: The customer’s estimated salary.
* Churn: The target variable, indicating whether the customer churned (1) or stayed (0).

## Steps of the Analysis
1. **Exploratory Data Analysis (EDA):**
   * Analyzed the distribution of numerical and categorical features.
   * Visualized the imbalance in the target variable (churn).
   * Identified and handled outliers and missing values (if applicable).

2. **Feature Engineering:**
   * Created new features like the balance-to-salary ratio and an indicator for senior customers.
   * Applied one-hot encoding to categorical features like gender and country.

3. **Model Selection:**
   * Evaluated three models: **Logistic Regression**, **Random Forest**, and **AdaBoost**.
   * Addressed the class imbalance using **class weights** to ensure the model focuses on both churn and non-churn cases.
  
4. **Performance Evaluation:**
   * The models were evaluated using key metrics like:
      * **Precision:** The accuracy of the positive (churn) predictions.
      * **Recall:** The proportion of actual churners that were correctly identified.
      * **F1-score:** The balance between precision and recall.
      * **ROC AUC:** The ability of the model to distinguish between churners and non-churners.
    
5. **Results**:
   * AdaBoost was the best-performing model with the following metrics:
       * **Precision:** 75% (When the model predicts churn, it's correct 75% of the time).
       * **Recall:** 50% (The model catches 50% of actual churners).
       * **F1-Score:** 0.60.
       * **ROC AUC:** 0.87, indicating strong overall performance in distinguishing churners from non-churners.

# **Conclusion**
AdaBoost was selected as the final model due to its ability to balance precision and recall, while achieving a strong ROC AUC score. This model provides a reliable way to predict churn and can be a valuable tool for the bank in its efforts to reduce customer loss.

# Future Work
* **Hyperparameter Tuning:** Further improvements could be made by fine-tuning the AdaBoost model’s parameters.
* **Larger Dataset:** Expanding the dataset or incorporating additional features could enhance the model’s predictive power.
* **Additional Models:** Other ensemble methods or deep learning models could be explored to improve performance.

## Requirements:
To run this project, the following Python packages are required:

pandas

numpy

scikit-learn

matplotlib

seaborn

LazyPredict

SweetViz




   
