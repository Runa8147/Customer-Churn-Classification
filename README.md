# Customer Churn Prediction

This project explores customer data and compares classification models for predicting whether a customer will churn.

## Dataset

The notebook uses `customer_churn_dataset-testing-master.csv`, which contains 64,374 customer records.

The available fields are:

- `CustomerID`
- `Age`
- `Gender`
- `Tenure`
- `Usage Frequency`
- `Support Calls`
- `Payment Delay`
- `Subscription Type`
- `Contract Length`
- `Total Spend`
- `Last Interaction`
- `Churn`

`Churn` is the target variable:

- `0`: No churn
- `1`: Churn

`CustomerID` is removed before model training because it is an identifier.

## Notebook Workflow

The notebook includes:

1. Loading and inspecting the dataset
2. Checking missing values and duplicate rows
3. Reviewing descriptive statistics and target distribution
4. Replacing negative numeric values with missing values
5. Exploratory visualizations for:
   - Contract length and churn
   - Tenure and churn
   - Subscription type and churn
   - Total spend and churn
6. Comparing numerical feature means by churn class
7. Separating features from the target
8. Splitting the data into training and testing sets
9. Encoding categorical features with one-hot encoding
10. Imputing missing values and scaling numerical features
11. Training and evaluating three classification models
12. Comparing model performance by F1 score

## Models

The following models are evaluated:

- Logistic Regression
- Decision Tree
- Random Forest

## Evaluation

Each model is evaluated using:

- Accuracy
- Precision
- Recall
- F1 score
- Classification report
- Confusion matrix

The model comparison table is sorted by F1 score in descending order.

## Tools Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## Project Structure

```text
semicolon/
├── churn_model.ipynb
├── churnmodel.py
├── customer_churn_dataset-testing-master.csv
├── requirements.txt
└── README.md
```

## How to Run

Install the required packages:

```bash
pip install -r requirements.txt
```

Open `churn_model.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab and run the cells in order. When using Google Colab, upload `customer_churn_dataset-testing-master.csv` when prompted.

Before running the notebook, correct the malformed `sklearn.metrics` import in the imports cell so that it uses the metric names listed in the notebook.

The standalone `churnmodel.py` file contains the dataset loading and initial inspection steps for a file named `customer_churn.csv`.
