# ETL for Interactive Brokers Data

## Overview

This project performs **Extract, Transform, Load (ETL)** operations on data from **Interactive Brokers (IBKR)** to facilitate the creation of **Global Investment Portfolios**. The primary objective is to **collect, process, and structure financial data** from multiple sources to support **investment decision-making**.

## Project Structure

The repository contains the following files:

| File                             | Description                                      |
| -------------------------------- | ------------------------------------------------ |
| `ETFS AMERICAS.csv`              | ETF data from the Americas region                |
| `ETFS APAC.csv`                  | ETF data from the APAC region                    |
| `ETFS EMEA.csv`                  | ETF data from the EMEA region                    |
| `INDICES AMERICAS EMEA APAC.csv` | Market indices from various global regions       |
| `STOCKS APAC.csv`                | Stock data from APAC countries                   |
| `STOCKS CANADA MEXICO.csv`       | Stock data from Canada and Mexico                |
| `STOCKS EMEA.csv`                | Stock data from EMEA countries                   |
| `STOCKS USA.csv`                 | Stock data from the United States                |
| `log_file.txt`                   | Log file for ETL process tracking                |
| `transformed_data.csv`           | Processed and cleaned dataset ready for analysis |

## Technologies Used

The project utilizes a variety of **tools, frameworks, and libraries** for data processing and analysis. Below are the key technologies used:

### Programming Language:
- ![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)

### Libraries & Frameworks:
- ![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-yellow) `pandas`
- ![Glob](https://img.shields.io/badge/Glob-File%20Handling-orange) `glob`
- ![Datetime](https://img.shields.io/badge/Datetime-Timestamp%20Handling-purple) `datetime`

### Cloud & Processing Tools:
- ![Google Colab](https://img.shields.io/badge/Google%20Colab-Cloud%20Notebooks-orange?logo=googlecolab)
- ![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-blue?logo=jupyter)

## Data Processing Steps

### 1. Extraction
- **Fetching raw data** from Interactive Brokers and other financial sources.
- Loading `.csv` files containing stock, ETF, and index data from global markets.

### 2. Transformation
- **Data Cleaning**: Handling missing values, removing outliers, and standardizing formats.
- **Feature Engineering**: Adding calculated fields.
- **Normalization**: Ensuring consistent data formats for further processing.

### 3. Loading
- Saving processed data into **structured `.csv` files** for analysis.

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/ETL_IBKR.git
   ```
2. Install dependencies:
   ```bash
   pip install pandas
   ```
3. Open `ETL_IBKR_DE_Global Investiments Portifolio.ipynb` in **Google Colab** or **Jupyter Notebook**.
4. Run the cells sequentially to execute the ETL process.

## Future Enhancements

- **Expand Data Sources**: Integrate more financial APIs for real-time updates.
- **Dashboard Development**: Build an interactive dashboard for investment insights.

## Contributing

Feel free to submit **pull requests** or **raise issues** for feature suggestions. Let’s build a **data-driven investment strategy together!**

## License

This project is licensed under the **MIT License**.

