# Customer Churn Prediction

AI/ML practical test project for predicting whether a customer is likely to churn based on customer information and service usage data.

## Objective

Build a classification model to predict customer churn and compare different machine learning approaches.

## Dataset

The dataset contains 64,374 customer records with information such as:

* Age
* Gender
* Tenure
* Usage Frequency
* Support Calls
* Payment Delay
* Subscription Type
* Contract Length
* Total Spend
* Last Interaction

The target variable is `Churn`:

* `0` – Not Churned
* `1` – Churned

`CustomerID` is excluded from model training as it is an identifier.

## Approach

The notebook covers:

1. Dataset loading and exploration
2. Data quality checking
3. Basic exploratory data analysis
4. Churn-related visualizations
5. Categorical feature encoding
6. Numerical feature preprocessing
7. Train-test split
8. Training multiple classification models
9. Model evaluation using:

   * Accuracy
   * Precision
   * Recall
   * F1 Score
   * Confusion Matrix
10. Model comparison and selection
11. Customer churn prediction
12. Churn probability estimation

## Machine Learning Models

The following classification models are compared:

* Logistic Regression
* Decision Tree
* Random Forest

## Results

The notebook contains the complete model evaluation, comparison, visualizations, observations, and prediction results.

## Project Structure

```text
customer-churn-prediction/
├── customer_churn.csv
├── Customer_Churn_Prediction.ipynb
└── README.md
```

## How to Run

Open `Customer_Churn_Prediction.ipynb` using Jupyter Notebook, JupyterLab, or Google Colab and run the cells sequentially.

## Tools Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
