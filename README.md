# Syntecxhub

Data Cleaning Utility 🧹
A robust, automated Python utility designed to clean messy datasets. This tool handles standardization, missing values, incorrect data types, and duplicates while generating a detailed audit log of every change made.

🚀 Features

Column Standardization: Converts all column names to snake_case and removes special characters for better coding compatibility. 


Duplicate Removal: Automatically detects and drops identical rows to ensure data uniqueness. 

Intelligent Type Casting:

Automatically identifies and converts numeric columns stored as text. 

Parses date columns using a 70% confidence threshold to avoid corrupting text data. 

Missing Value Imputation:


Numerical Columns: Fills missing values with the Mean. 


Categorical Columns: Fills missing values with the Mode (most frequent value). 


Audit Logging: Generates a cleaning_log.txt file that records every action taken during the process for full transparency. 

🛠️ Tech Stack
Language: Python

Library: Pandas, NumPy

Environment: Jupyter Notebook 

📁 Project Structure
Plaintext
├── DATA_SEICNCE/
│   └── train.csv          # Original raw dataset
├── cleaned_data.csv       # Final output (generated after running)
├── cleaning_log.txt       # Audit report (generated after running)
└── data_cleaning.ipynb    # Main project script
📖 How It Works
Standardization: The utility strips whitespace and replaces spaces with underscores in column headers.

Dtype Fix: It checks if a column should be a number or a date and converts it accordingly.

Handling Nulls: It applies statistical imputation so you don't lose rows of data.


Reporting: A summary is printed to the console and saved to a text file. 

