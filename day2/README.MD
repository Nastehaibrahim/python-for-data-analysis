# Data Cleaning & Transformation with Pandas

This project demonstrates core data manipulation, subsetting, and filtering techniques using the Python `pandas` library on student enrollment data.

---

## 📌 Features & Key Operations

* **Data Ingestion**: Loading Excel datasets via `pd.read_excel()`[cite: 2]
* **Column Selection**: Extracting single or multiple features (e.g., `Program`, `Gender`)[cite: 2]
* **Label & Integer Indexing**:
  * Selecting specific rows and columns using `.loc[]`[cite: 2]
  * Positional slicing using `.iloc[]`[cite: 2]
* **Data Cleaning**: Type casting non-numeric fields using `pd.to_numeric(..., errors='coerce')`[cite: 2]
* **Data Filtering**:
  * Numerical filtering based on conditional criteria[cite: 2]
  * Categorical filtering using standard equality and `.isin()`[cite: 2]
  * Complex multi-condition filtering with logical operators (`&`, `|`)[cite: 2]
* **Data Sorting**: Ordering datasets by specific columns using `.sort_values()`[cite: 2]

---

## 🛠️ Code Examples

```python
import pandas as pd

# Load dataset
data = pd.read_excel("path_to_dataset.xlsx")

# Select specific columns
program_gender = data[['Program', 'Gender']]

# Filter data for specific categories
female_students = data[data['Gender'] == 'Female']

# Convert column to numeric and filter values
data['Tuition_Fee'] = pd.to_numeric(data['Tuition_Fee'], errors='coerce')
low_tuition = data[data['Tuition_Fee'] < 1000]

# Multi-condition filter
filtered_data = data[(data['Gender'] == 'Female') & (data['Tuition_Fee'] < 1000)]

# Sort values
sorted_data = data.sort_values('Tuition_Fee')
