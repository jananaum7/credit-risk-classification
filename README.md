# Credit Risk Classification

## Table of Contents
1. [Getting Started](#getting_started)
2. [Introduction](#introduction)
3. [Credit Risk Analysis Report](#credit_risk_analysis_report)
4. [Contributers](#contributers)

## Getting Started
   - Clone the Repository: Open Git Bash and navigate to the directory where you want to store the project. Use the following command to clone the repository:
     - ``` bash
         git clone git@github.com:jananaum7/credit-risk-classification.git
        ```
   - Navigate to the Project Directory: Change into the newly created project directory:
     - ``` bash
       cd credit-risk-classification
       ```
   - Create the credit_risk Folder: Inside the credit-risk-classification, create a new folder named Credit_Risk:
     - ``` bash
       mkdir Credit_Risk
       ```
   - Add Starter Code and Resources: Place your starter code and any necessary resources into the credit_risk folder.

## Introduction
In this assignment, I developed a **Credit Risk Classification** model using **Logistic Regression** to predict whether a loan is **high-risk (1)** or **healthy (0)**. The aim was to create a model that helps evaluate the likelihood of a borrower defaulting on a loan. The model was trained on a loan dataset and evaluated using various performance metrics.

## Credit Risk Analysis Report
* Purpose of the analysis
  - The purpose of this analysis was to develop a Credit Risk Classification model that predicts whether a loan is high-risk (1) or healthy (0). 
* Financial Information & Prediction Goals
  - The data contains information about different loans, including details like the loan size, interest rates, and borrower information. The main goal of this analysis was to predict whether each loan is high-risk (1) or healthy (0). Accurately making these predictions 
    is crucial for minimizing financial losses by identifying which loans are more likely to fail.
* Target Variable Overview
  - The variable I was trying to predict is whether a loan is high-risk (1) or healthy (0). Here's the breakdown of the values:
    - `0` (Healthy loans): **18,765**  
    - `1` (High-risk loans): **619**  
  - This showcases that the data is **imbalanced**, with far more `healthy loans` than `high-risk loans`.
* Stages of the Machine Learning Process
  - Data Preparation:
    - Read the CSV file from the Resources folder into Pandas and reviewed the data frame. 
  - Creating Features and Target Variables:
    - I created the labels set (y) from the “loan_status” column, and then created the features (X) DataFrame from the remaining columns. I then reviewed both the x and y variable.
  - Data Splitting:
    - I split the data into training and testing datasets by using `train_test_split`.
  - Logistic Regression Model:
    - Created a Logistic Regression Model with the Original Data
      - Fit a logistic regression model by using the training data (`X_train` and `y_train`).
      - Saved the predictions on the testing data labels by using the testing feature data (`X_test`) and the fitted model.
  - Evaluating Model Performance:
    - Evaluated the model’s performance by doing the following.
      - Created a confusion matrix
      - Printed the classification report
* Machine Learning Model: Logistic Regression: 
The model worked well overall, especially in predicting healthy loans (`0`). It performed a bit worse with high-risk loans (`1`), because there are fewer high-risk loans in the data. Precision and recall showcased the model was good at identifying healthy loans, but less accurate with high-risk ones due to the imbalance in the dataset.
* Results:
  - The model had a very high accuracy, correctly predicting healthy and high-risk loans in almost all cases.
  - The precision for high-risk loans was strong, meaning when the model predicted a loan as high-risk, it was usually correct.
  - The recall for high-risk loans was also high, indicating the model was good at identifying most of the true high-risk loans.
* Summary
  - The logistic regression model performed well overall, accurately predicting healthy loans and identifying most high-risk loans. However, due to the class imbalance—where healthy loans are more common—the model was slightly less effective at detecting high-risk 
    loans. This means it occasionally missed some high-risk loans or incorrectly labeled healthy loans as high-risk. Despite this, the model's strong performance in predicting healthy loans indicates its effectiveness in identifying low-risk loans.

## Contributers 
   - J. Naum
   - Minor error corrections and README improvements were assisted by [ChatGPT](https://openai.com/chatgpt) and Xpert learning assistant. 
