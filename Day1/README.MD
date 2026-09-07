# Airline Data Analysis & Exploration

This repository contains a Python notebook focused on loading and exploring dataset information for airline/project records using **pandas**.

---

## 🛠️ Requirements & Tools

* **Python 3.x**
* **Pandas** (`pip install pandas`)
* **OpenPyXL** (Required for reading Excel files: `pip install openpyxl`)

---

## 🚀 Key Steps in the Notebook

* **Library Import:** Imports `pandas` as `pd`.
* **Data Loading:** Loads the Excel file (`airline project.xlsx`) into a pandas DataFrame.
* **Data Exploration:**
  * Checks dataset dimensions using `Data.shape`.
  * Inspects leading rows (`Data.head(10)`) and trailing rows (`Data.tail(5)`).
  * Lists column names using `Data.columns`.
  * Inspects data types using `Data.dtypes`.
  * Summarizes metadata using `Data.info()`.
  * Generates summary statistics using `Data.describe()`.

---

## 📋 Code Snippets

```python
# Import library
import pandas as pd

# Load dataset
data = pd.read_excel("airline project.xlsx")

# Explore structure
print(data.shape)
print(data.head())
print(data.info())
