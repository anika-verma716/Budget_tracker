# Personal Budget Tracker

## 1. Project Overview

The Personal Budget Tracker is a Python-based data analysis project that helps users understand and manage their income and expenses.

The project uses a financial transaction dataset to calculate total income, total expenses, net savings, category-wise spending, and monthly expenses. It also includes a budget management feature that allows users to enter a monthly budget and check whether their expenses are within the budget.

The project is developed using Python and its data analysis libraries. It provides text-based reports without graphical visualizations.

## 2. Project Objectives

The main objectives of this project are:

- To analyze personal income and expenses.
- To calculate total income, total expenses, and net savings.
- To identify the highest spending category.
- To analyze monthly expenditure patterns.
- To help users monitor their monthly budget.
- To identify whether expenses exceed the available budget.
- To practice data cleaning, data analysis, and Python programming.

## 3. Technologies Used

The following technologies and libraries are used:

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Pandas | Data cleaning, manipulation, and analysis |
| NumPy | Numerical operations |
| Google Colab | Cloud-based development environment |
| Kaggle | Source of the financial dataset |
| GitHub | Project storage and version control |

## 4. Dataset

**Dataset Name:** `expense_data_1.csv`

**Dataset Source:** Kaggle

The project uses a personal expense and income transaction dataset containing 277 transactions and 11 original columns.

The dataset includes information such as:

- Date
- Account
- Category
- Subcategory
- Note
- Income/Expense
- Amount
- Currency

### Data Preprocessing

Before analysis, the dataset undergoes the following cleaning steps:

1. Removing unnecessary columns.
2. Removing duplicate records.
3. Converting the Date column into datetime format.
4. Converting Amount into numeric format.
5. Handling missing values.
6. Cleaning category and transaction-type names.

After preprocessing, the cleaned dataset contains 7 columns.

## 5. Key Features

### 1. Dataset Information
Displays the total number of transactions and categories.

### 2. Financial Summary
Calculates:
- Total Income
- Total Expenses
- Net Savings

### 3. Category-Wise Expense Analysis
Calculates the total amount spent in each expense category and identifies the highest spending category.

### 4. Monthly Expense Analysis
Displays month-wise expenses and identifies the month with the highest expenditure.

### 5. Budget Management
Allows users to:
- Enter a monthly budget.
- Select a month in YYYY-MM format.
- Calculate total expenses for that month.
- Calculate the remaining budget.
- Receive a warning if expenses exceed the budget.

## 6. How to Run the Project

Follow these steps to run the project:

**Step 1: Open Google Colab**

Visit Google Colab and create a new notebook.

**Step 2: Install Required Libraries**

Run the following command:

```python
!pip install pandas numpy
```

**Step 3: Upload the Dataset**

Upload the `expense_data_1.csv` file to Google Colab.

**Step 4: Import Libraries**

```python
import pandas as pd
import numpy as np
```

**Step 5: Load the Dataset**

```python
df = pd.read_csv('expense_data_1.csv')
```

**Step 6: Execute the Code**

Run the remaining project code cells in sequence to perform data cleaning, financial analysis, category-wise analysis, monthly analysis, and budget management.

**Step 7: Use Budget Management**

Enter your monthly budget and the required month in YYYY-MM format when prompted.

The program will generate a budget report showing total expenses and the remaining budget.

## 7. Sample Output

### Financial Summary

```text
========== PERSONAL BUDGET TRACKER ==========

Total Transactions: 277

Total Income: Rs. 54754.00
Total Expenses: Rs. 57918.28
Net Savings: Rs. -3164.28
```

### Budget Management

```text
========== BUDGET REPORT ==========

Selected Month: 2022-01
Monthly Budget: Rs. 15000.0
Total Expenses: Rs. 20679.51
Remaining Budget: Rs. -5679.51

WARNING! You have exceeded your budget.
Extra Spending: Rs. 5679.51

===================================
```

*Note: The sample output is based on the transactions available in the Kaggle dataset.*

## 8. Project Limitations

- The analysis depends on the transactions available in the uploaded dataset.
- The dataset contains historical transactions rather than live financial data.
- The project currently provides text-based reports.
- Budget calculations are based on the selected month's recorded expenses.

## 9. Future Improvements

The project can be enhanced by adding:

- Manual transaction entry.
- Data storage for new transactions.
- Monthly income and savings analysis.
- Exportable financial reports.
- A graphical user interface.

## 10. Author

**Author:** [Your Name]

**Project:** Personal Budget Tracker

**Domain:** Data Analytics

**Programming Language:** Python
