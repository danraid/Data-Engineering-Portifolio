# 📊 Banks ETL Project

## 📌 Project Overview
This project aims to extract, transform, and load (ETL) data related to the **largest banks in the world** ranked by market capitalization. The extracted data is transformed into multiple currencies using exchange rate data and stored in a structured format for further analysis.

## 🛠️ Technologies & Tools Used

### Programming Language
- ![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)

### Libraries & Frameworks
- ![Requests](https://img.shields.io/badge/Requests-Web%20Scraping-blue) `requests`
- ![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-HTML%20Parsing-green) `bs4`
- ![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-yellow) `pandas`
- ![SQLite](https://img.shields.io/badge/SQLite-Database-lightgrey) `sqlite3`
- ![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-orange) `numpy`
- ![Datetime](https://img.shields.io/badge/Datetime-Timestamp%20Handling-purple) `datetime`

## 📂 Project Structure
```
├── Banks_ETL_Project.ipynb  # Jupyter Notebook with full ETL implementation
├── exchange_rate.csv        # Exchange rates data
├── Largest_banks_data.csv   # Processed dataset with transformed values
├── Banks.db                 # SQLite database storing the final table
├── code_log.txt             # Log file for tracking process execution
├── README.md                # Project documentation
```

## 🚀 ETL Process
### 1️⃣ Extraction (Extract)
- Web scrapes the **Wikipedia** page (archived version) to extract the top **10 largest banks** ranked by market capitalization.
- Extracted attributes: `Name`, `MC_USD_Billion`

### 2️⃣ Transformation (Transform)
- Converts **market capitalization (USD)** to **GBP, EUR, and INR** using exchange rates.
- Rounds values for readability.

### 3️⃣ Loading (Load)
- Saves the transformed data in a **CSV file**.
- Loads the final table into an **SQLite database**.

## 📊 SQL Queries Executed
- **Retrieve all bank records:**
  ```sql
  SELECT * FROM Largest_banks;
  ```
- **Calculate the average market capitalization in GBP:**
  ```sql
  SELECT AVG(MC_GBP_Billion) FROM Largest_banks;
  ```
- **List the top 5 banks:**
  ```sql
  SELECT Name FROM Largest_banks LIMIT 5;
  ```

## 📑 Log File (`code_log.txt`)
- Logs progress at every stage (extraction, transformation, loading, SQL execution).

## 📥 Notebook Download
📎 [Banks_ETL_Project.ipynb](./Banks_ETL_Project.ipynb)

