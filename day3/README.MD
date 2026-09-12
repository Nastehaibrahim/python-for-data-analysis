# Data Cleaning ✈️

This project focuses on cleaning and formatting airline booking data using **Python** and **Pandas**.

## 📌 Data Cleaning Steps

* **Column Renaming:** Renamed the `BKGID` column to `Booking_ID` for clarity.
* **Text Consistency & Formatting:**
  * **`Travel_Class`**: Applied `.str.lower()` to standardize class entries (e.g., Economy, Business).
  * **`Route`**: Applied `.str.strip()` to remove whitespace and `.str.upper()` to standardize airport codes.
  * **`Booking_Status`**: Applied `.str.title()` to clean up status values (e.g., Completed, Confirmed, Cancelled).
* **Data Type Conversions:**
  * **`Ticket_Price`**: Converted to numeric values using `pd.to_numeric()`.
  * **`Flight_Date`**: Converted to datetime objects using `pd.to_datetime()`.

---

## 🛠️ Technologies Used

* **Python 3**
* **Pandas**
