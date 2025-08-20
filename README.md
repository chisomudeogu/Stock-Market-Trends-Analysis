**Stock Market Trend Dashboard Project**

**Author:** Chisom Chinedu-Onuoha

**Date:** August 2025

**1. Aim of the Project**

To develop an interactive Power BI dashboard that analyzes and visualizes stock market trends for both international and Nigerian stocks, enabling stakeholders to monitor performance, compare sectors, and identify investment opportunities.
The project also aims to demonstrate data analytics and visualization skills using real-world financial data collected via Python and multiple APIs/data sources.

**2. Objectives**

- Collect and process daily stock price data for selected 10 international stocks and 5 Nigerian stocks from January 1, 2020, to present.
- Integrate key metrics such as:
      Daily returns
      Cumulative returns
      50-day & 200-day moving averages
- Combine all data into a single clean dataset for Power BI visualization.
- Design a dashboard with:
      International & Nigerian stock performance comparison
      Sector-wise analysis
      Technical trend indicators
      Provide actionable insights for investors and analysts.

**3. Tools and Technologies**
- Python (Data collection, cleaning, processing)
- yfinance – for international stock data
- pandas – for data manipulation
- glob – for reading multiple CSVs
- datetime – for date handling
- Investing.com – manual download of Nigerian stock data (CSV format)
- Google Colab – cloud-based Python environment
- Google Drive – file storage and sharing
- Power BI Desktop – data visualization and dashboard creation

**4. Data Sources**

**International Stocks (10 tickers) — via Yahoo Finance API (yfinance):**

- AAPL (Apple Inc.)
- MSFT (Microsoft Corporation)
- TSLA (Tesla Inc.)
- AMZN (Amazon.com Inc.)
- GOOG (Alphabet Inc.)
- META (Meta Platforms Inc.)
- NVDA (NVIDIA Corporation)
- JPM (JPMorgan Chase & Co.)
- XOM (Exxon Mobil Corporation)
- BRK-B (Berkshire Hathaway Inc.)

**Nigerian Stocks (5 tickers) — downloaded from Investing.com:**

- GTCO (Banking)
- ZENITHBANK (Banking)
- MTNN (Telecoms)
- DANGCEM (Industrial)
- AIRTELAFRI (Telecoms)

**5. Methodology**

**Step 1  Data Collection**
- Used yfinance to programmatically download daily historical data for global stocks from Jan 1, 2020, to the current date.
- Manually downloaded CSV files for Nigerian stocks from Investing.com from Jan 1, 2020 to August 13, 2025
- Stored Nigerian stock files in a dedicated Google Drive folder.

**Step 2  Data Cleaning**

For international stocks:
- Extracted price data
- Calculated daily returns, cumulative returns, and moving averages (50-day & 200-day)

For Nigerian stocks:
- Renamed columns to match international dataset
- Removed commas in numeric columns and converted to floats
- Calculated the same metrics as for international stocks
- Ensured all Date fields were in datetime format.

**Step 3  Data Integration**
- Combined both datasets into a single DataFrame in Python.
- Saved as combined_stock_data.csv.

**Step 4  Data Validation**
- Checked for missing values, duplicates, and date alignment.
- Verified that metrics calculated in Python matched spot checks from original data sources.

**6. Results (Dashboard Pages)**
**Page 1:** Market Overview → KPIs (Top/Worst Stocks, Avg Daily Return), Trend charts, slicers by country & ticker.
**Page 2:** Sector Performance → Avg cumulative return by sector, Heatmap by sector/date, KPIs for best/worst sectors.


**7. Insights (Interpretations)**
1. Overall & International Market Overview
- Top Performing Stock → NVIDIA (+2,967%) — this is fueled by AI & semiconductor demand.
- Worst Performing Stock → ExxonMobil (+94%) — energy sector lagged due to oil price volatility and global transition to renewables.

**Notable Trends:**
Tech dominance (AAPL, MSFT, GOOG, META) — stock prices here show a generally strong upward momentum, with temporary dips around 2022 for GOOG and META.
E-commerce (AMZN) — volatile: pandemic growth in 2021, slump in 2022–2023, recovery in 2024–2025.
Financials (JPM) — cyclical, hit in 2022, recovery afterward.
Conglomerates (BRK-B) — stable and consistently upward.

2. Nigerian Market Overview
- Top Performing Stock → Airtel Africa (+694%) — strong growth from telecom demand and digital adoption.
- Worst Performing Stock → GTCO (+239%) — still positive but lagging banking peers due to sector challenges.

Trends:
Telecoms (MTNN, Airtel) — high growth sector, reflecting Nigeria’s digital expansion.
Banking (GTCO, Zenith) — modest growth, pressured by FX volatility and regulations.
Dangote Cement — strong industrial play but weakened in 2025.

3. Sector Performance
- Best Performing Sector (Global) → Semiconductors (+2,967%), driven by NVDA.
- Best Performing Sector (Nigeria) → Telecoms (+673%), led by Airtel.
- Worst Performing Sector (Global) → Energy (+94%), underperformed amid oil shocks and transition to renewables.
- Worst Performing Sector (Nigeria) → Banking (+239%), slower returns compared to telecoms & industrials.

Heatmap Patterns
Automotive and E-commerce struggled in 2022, showing how some sectors are easily hit by shocks.
Tech and Semiconductors bounced back strongly after 2022, proving their resilience.
By 2025, Nigeria’s Banking and Industrial sectors stayed strong while some global sectors slowed down.

** 8. Value to Stakeholders**

For Investors: Clear identification of outperforming sectors (Semiconductors, Telecoms) vs laggards (Energy, Banking) for better portfolio allocation.
For Hiring Managers: This project demonstrates data collection, integration of multiple sources, cleaning, Python scripting, Power BI dashboarding, and insight storytelling.
For General Audiences: This is an easy-to-understand dashboard showing how global vs Nigerian markets have performed side-by-side.

Summary:
Between 2020–2025, Technology (esp. Semiconductors) and Telecoms emerged as the international and Nigerian growth leaders. Energy (international) and Banking (Nigeria) underperformed, reflecting sector-specific challenges. The analysis shows how different economies and industries respond to global shocks, highlighting opportunities for diversification.

**9. Skills Demonstrated**
- Data sourcing (API & manual)
- Data cleaning and transformation in Python
- Time series analysis
- Financial metrics calculation
- Data integration from multiple sources
- Interactive dashboard design in Power BI




