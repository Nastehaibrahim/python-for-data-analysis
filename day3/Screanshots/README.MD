# Airline Booking Data Cleaning & Preprocessing ✈️

This repository contains a comprehensive data cleaning and preprocessing pipeline for an airline booking dataset using **Python** and **Pandas**. The project focuses on handling missing values, standardizing column data types, and cleaning text fields for accurate downstream analysis.

---

## 📌 Key Data Cleaning Steps

1. **Column Renaming & Removal**
   * Renamed identifier columns (`BKGID` → `Booking_ID`) to improve data readability.
   * Dropped redundant or unnecessary columns using `data.drop()`.

2. **Data Type Conversion**
   * **`Ticket_Price`**: Parsed string values to numeric representations using `pd.to_numeric(..., errors='coerce')`.
   * **`Flight_Date`**: Converted raw date entries into datetime objects via `pd.to_datetime(..., errors='coerce')`.

3. **String Standardization & Formatting**
   * **`Route`**: Applied `.str.strip()` to strip leading/trailing whitespace and `.str.upper()` to enforce consistent uppercase airport codes (e.g., `MGQ-NBO`, `MGQ-ADD`).
   * **`Travel_Class`**: Standardized string casing using `.str.lower()` and `.replace()` to fix inconsistent class categories.
   * **`Booking_Status`**: Normalized categorical values (e.g., `Completed`, `Confirmed`, `Cancelled`) using `.str.title()`.

---

## 🛠️ Technologies & Libraries

* **Python 3**
* **Pandas** (Data Manipulation & Preprocessing)
* **Jupyter / Google Colab** Notebook Environment

   ```bash
   git clone [https://github.com/Nastehaibrahim/python-for-data-analysis.git](https://github.com/Nastehaibrahim/python-for-data-analysis.git)
