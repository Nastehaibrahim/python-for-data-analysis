# Data Cleaning & Transformation with Pandas

This project demonstrates core data manipulation, subsetting, and filtering techniques using the Python `pandas` library on student enrollment data.

---

## 📌 Features & Key Operations

* **Data Ingestion**: Loading Excel datasets via `pd.read_excel()`
* **Column Selection**: Extracting single or multiple features (e.g., `Program`, `Gender`)
* **Label & Integer Indexing**:
  * Selecting specific rows and columns using `.loc[]`
  * Positional slicing using `.iloc[]`
* **Data Cleaning**: Type casting non-numeric fields using `pd.to_numeric(..., errors='coerce')`
* **Data Filtering**:
  * Numerical and categorical condition filtering
  * Multi-category matching via `.isin()`
  * Multi-condition boolean logic (`&`, `|`)
* **Sorting**: Ordering DataFrames based on numerical columns (e.g., `Tuition_Fee`)

---

## 🛠️ Requirements & Installation

Make sure you have Python installed along with `pandas` and `openpyxl` (for reading Excel files):
                                                                        import pandas as pd

# Load dataset
data = pd.read_excel("python dataset.xlsx")

# Convert column to numeric (coercing errors)
data['Tuition_Fee'] = pd.to_numeric(data['Tuition_Fee'], errors='coerce')

# Filter for female students with specific conditions
female_students = data[data['Gender'] == 'Female']

# Display first few rows
print(female_students.head())
📂 Dataset Schema
The notebook analyzes a dataset containing the following fields:

Student_ID

Gender

Program

Enrollment_Date

Study_Mode

Tuition_Fee

Enrollment_Status
                                                                        

                                                                        

```bash
pip install pandas openpyxl
