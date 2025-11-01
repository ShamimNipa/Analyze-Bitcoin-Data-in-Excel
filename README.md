# Analyze-Bitcoin-Data-in-Excel
This project is an analysis of Bitcoin price data using the Excel skills 
# Cryptocurrency Data Analysis: Upside and Volatility

## Project Overview
This project analyzes the potential upside and volatility of various cryptocurrency symbols (e.g., Bitcoin, Ethereum) for the year 2021. The goal is to provide insights into price performance, risk, and potential investment recommendations.

The analysis involves:
- Cleaning and preparing text, date, and numeric data.
- Calculating percentage gains (upside) over 2021.
- Analyzing volatility through daily high/low spreads.
- Creating pivot tables and visualizations to summarize trends.
- Providing a final recommendation based on the balance between upside and risk.

---

## Dataset
The dataset contains daily cryptocurrency prices and other relevant metrics.

**Columns include:**
| Column Name | Description |
|-------------|-------------|
| Date        | Trading date (YYYY-MM-DD) |
| Symbol      | Cryptocurrency ticker (e.g., BTC, ETH) |
| Open        | Opening price |
| High        | Highest price of the day |
| Low         | Lowest price of the day |
| Close       | Closing price |
| Volume      | Trading volume |
| Market Cap  | Market capitalization |

**Additional derived/cleaned columns:**
| Column Name | Description |
|-------------|-------------|
| Symbol_Trimmed | Cleaned Symbol column (no extra spaces) |
| Month        | Extracted month for pivot tables (YYYY-MM) |
| First_2021_Open | First opening value in 2021 (Upside sheet) |
| Last_2021_Close | Last closing value in 2021 (Upside sheet) |
| Percent_Change | Upside percentage over 2021 |
| Largest_High | Maximum daily high for each symbol (Spread sheet) |
| Smallest_Low | Minimum daily low for each symbol (Spread sheet) |
| Low_as_Percent_of_High | Measure of volatility |

---

## Analysis Steps

1. **Data Cleaning**
   - Trim whitespace from text columns.
   - Check for missing or blank entries in text, numeric, and date columns.
   - Inspect date and numeric columns for suspect values.

2. **Upside Analysis**
   - Calculate first 2021 open and last 2021 close for each symbol.
   - Compute the percentage change:  
     ```
     Percent Change = (Last Close - First Open) / First Open
     ```
   - Visualize results with a bar chart.

3. **Volatility Analysis**
   - Identify the largest high and smallest low for each symbol.
   - Calculate volatility as:
     ```
     Low as % of High = Smallest Low / Largest High
     ```
   - Visualize with a bar chart.

4. **Exploratory Data Analysis**
   - Create pivot tables to analyze average monthly closing prices per symbol.
   - Apply color scales (red-low to green-high) individually to columns.
   - Create pivot tables for daily highs per symbol with line charts.

5. **Final Recommendation**
   - Compare upside potential vs. volatility.
   - Provide investment guidance based on risk tolerance.

---

## Visualizations
- **Upside Bar Chart:** Shows the percentage change for each symbol over 2021.
- **Volatility Bar Chart:** Shows the relative risk (low as % of high) for each symbol.
- **Line Chart:** Daily highs per symbol over time.
- **Conditional Formatting:** Red-to-green color scales to highlight trends in numeric data.

---

## Tools Used
- **Excel** for data cleaning, pivot tables, formulas, and visualizations.

---

## Usage
1. Open the Excel workbook.
2. Navigate through the sheets:
   - `Upside` → Analyze potential gains.
   - `Spread` → Analyze volatility.
   - `Exploratory Data Analysis` → Monthly average trends.
   - `Daily Highs` → Daily maximum prices and line charts.
   - `Final Recommendation` → Summary of findings and investment guidance.
3. Refresh pivot tables if the dataset is updated.

---

## Notes
- Some missing data (e.g., SP500 on weekends) is expected.
- Suspect values should be checked before analysis; this project assumes the dataset is clean.
- Recommendations are based solely on historical 2021 data and do not predict future performance.

---

## Author
[Nipa]  
[Date]

