# 📊 Data Cleaning & Transformation with Pandas

Welcome to the **Data Cleaning & Transformation** repository! This project covers fundamental-to-intermediate data manipulation, subsetting, and filtering techniques using Python's `pandas` library on student enrollment data.

---

## 📌 Features & Key Operations

* **Data Ingestion**: Reading dataset files via `pd.read_excel()`.
* **Column Selection**: Extracting single or multiple attributes (e.g., `Program`, `Gender`).
* **Label & Integer Slicing**:
  * Selecting specific rows and columns with `.loc[]`.
  * Positional indexing with `.iloc[]`.
* **Data Cleaning & Conversion**: Enforcing numeric data types using `pd.to_numeric(..., errors='coerce')`.
* **Conditional Filtering**:
  * Filtering by numerical thresholds and categorical values.
  * Matching multiple categories using `.isin()`.
  * Applying logical conditions (`&`, `|`).
* **Data Sorting**: Ordering DataFrames by numerical features like `Tuition_Fee`.

---

## 📸 Code Walkthrough

### 1. Data Ingestion & Single Column Selection
Loading the dataset and viewing specific series columns:

```python
import pandas as pd

# Load dataset
data = pd.read_excel("/content/drive/MyDrive/Colab Notebooks/python dataset.xlsx")
# Select multiple columns
data[['Program', 'Gender']]
# Select a single column# Select rows using label indexing
data.loc[0:5]
# Select multiple columns
data[['Program', 'Gender']]
data.iloc[0:3]# Select rows using label indexing
data.loc[0:5]

# Select rows and specific columns using loc
data.loc[0:5, ['Program', 'Gender']]

# Select rows using integer positional indexing
data.iloc[0:3]# Convert Tuition_Fee to numeric, coercing non-numeric string values to NaN
data['Tuition_Fee'] = pd.to_numeric(data['Tuition_Fee'], errors='coerce')

# Filter rows based on numerical threshold
data[data['Tuition_Fee'] < 10]# Categorical filtering
data[data['Gender'] == 'Female']

# Filtering multiple categories using .isin()
data[data['Gender'].isin(['Female', 'NAN'])]

# Multi-condition boolean logic
data[(data['Gender'] == 'Female# Sort records by Tuition Fee
data.sort_values('Tuition_Fee')') & (data['Tuition_Fee'] < 20)]
data['Gender']
