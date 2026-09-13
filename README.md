📊 S&P 500 Stock Market Analysis Dashboard Using Power BI

An interactive Power BI financial analytics project built to analyze S&P 500 companies, historical stock prices, trading volume, company performance, sector distribution, and long-term market trends.

🚀 Project Overview

The project uses two datasets:

sp500_companies — company-level information for 503 companies

sp500_stocks — more than 1 million historical stock records

The stock data covers 3 January 2000 to 30 July 2026, providing approximately 25+ years of historical market data.

The dashboard is designed to help users explore stock-market trends through interactive company, sector, symbol, and date filters.

🎯 Objectives

Analyze historical S&P 500 stock-price movements.

Study Open, High, Low, and Close prices.

Analyze trading volume over time.

Compare companies based on average closing price.

Analyze the distribution of companies across sectors.

Identify companies with high average historical closing prices.

Study long-term market behavior over 25+ years.

Build interactive and business-friendly Power BI dashboards.

📑 Dashboard Pages

1. 🏠 S&P 500 Stock Market Dashboard

The main dashboard provides a high-level overview of the S&P 500 dataset.

KPI Cards

Total Companies: 503

Average Close: 73.32

Highest Price: 4,388.11

Total Trading Volume: approximately 8.50 trillion shares

Visuals

Stock Closing Price Trend

Company by Sector

Trading Volume Over Time

Top 10 Companies by Average Closing Price

Symbol, Company, Sector, and Date slicers

Main DAX Measures

Total Companies =
DISTINCTCOUNT(sp500_companies[Symbol])

Average Close =
AVERAGE(sp500_stocks[close])

Highest Price =
MAX(sp500_stocks[high])

Total Volume =
SUM(sp500_stocks[volume])

2. 📈 Company Stock Analysis

This dashboard page is focused on analyzing individual companies and their historical stock performance.

Users can select a company/symbol and investigate its stock-price behavior across the available date range.

Analysis Areas

Opening Price

Closing Price

Highest Price

Lowest Price

Trading Volume

Historical price movement

Company-level performance comparison

Date-based analysis

This page helps users move from the overall S&P 500 view to detailed company-level analysis.

3. 🏢 Sector Analysis

The Sector Analysis dashboard focuses on comparing the S&P 500 across its major business sectors.

11 Sectors

Industrials

Financials

Information Technology

Health Care

Consumer Discretionary

Consumer Staples

Utilities

Real Estate

Materials

Communication Services

Energy

Analysis Areas

Number of companies by sector

Sector-wise stock performance

Sector comparison

Trading activity

Historical sector trends

According to the dataset, the largest sectors by company count include Industrials (81), Financials (76), and Information Technology (74).

4. 📅 25-Year S&P 500 Market Analysis

This page focuses on long-term market behavior using historical data beginning in 2000.

Historical Periods

2000–2002

Study market conditions following the technology-sector downturn.

2007–2009

Analyze the impact of the global financial crisis.

2010–2019

Explore long-term market growth and increasing technology-sector importance.

2020

Analyze significant market volatility during the COVID-19 period.

2021 onwards

Explore market recovery and more recent stock-market movements.

The Date slicer allows users to select different periods and compare price trends and trading activity.

🗂️ Dataset Description

sp500_companies

Contains information about 503 S&P 500 companies.

Important columns:

Column

Description

Symbol

Stock ticker symbol

Company

Company name

Sector

Main business sector

Sub_Industry

Detailed industry classification

Head_Quarters

Company headquarters

Date_Added

Date added to S&P 500

Founded

Company founding information

sp500_stocks

Contains 1,048,575 historical stock records.

Important columns:

Column

Description

Date

Trading date

Open

Opening stock price

High

Highest price during the trading day

Low

Lowest price during the trading day

Close

Closing stock price

Volume

Number of shares traded

Symbol

Stock ticker symbol

🔗 Data Model

The two datasets are connected through the stock symbol:

sp500_companies[Symbol]
          │
          │ One-to-Many
          ▼
sp500_stocks[symbol]

One company record can be connected to many daily stock records.

This relationship allows company and sector information to interact with historical stock data.

📊 Key Visualizations

Stock Closing Price Trend

A line chart showing the average closing price over time.

Company by Sector

A donut chart showing the distribution of companies across the 11 sectors.

Trading Volume Over Time

A clustered column chart showing changes in trading activity across the historical period.

Top 10 Companies

A clustered bar chart showing the Top 10 companies by average closing price.

🎛️ Interactive Filters

The dashboard includes:

Symbol

Company

Sector

Date Range

These filters allow users to interactively explore different companies, sectors, and historical periods.

🛠️ Tools & Technologies

Power BI

DAX

Power Query

Excel / CSV

Data Cleaning

Data Modeling

Data Visualization

KPI Development

Time-Series Analysis

Financial Data Analysis

📌 Key Insights

The dataset contains 503 companies across 11 sectors.

The stock dataset contains more than one million historical records.

Historical data begins in January 2000.

The project enables long-term analysis over approximately 25+ years.

Industrials, Financials, Information Technology, and Health Care have significant representation.

Combining company information with daily stock data enables company-level and sector-level analysis.

Interactive filters make it easier to investigate specific companies, sectors, and periods.

🖼️ Dashboard Preview

Add the dashboard screenshot to your repository, for example:

assets/
└── sp500-dashboard.png

Then add it to this README:

![S&P 500 Power BI Dashboard](assets/sp500-dashboard.png)

📁 Suggested GitHub Repository Structure

S&P-500-Stock-Market-Analysis/
│
├── README.md
│
├── Dashboard/
│   └── S&P_500_Stock_Market_Analysis.pbix
│
├── Dataset/
│   ├── sp500_companies.csv
│   └── sp500_stocks.csv
│
├── assets/
│   └── sp500-dashboard.png
│
└── Documentation/
    └── Project_Details.md

💡 Skills Demonstrated

This project demonstrates practical skills in:

Data Cleaning

Data Transformation

Data Modeling

One-to-Many Relationships

DAX

Power Query

KPI Creation

Data Visualization

Interactive Dashboard Design

Time-Series Analysis

Financial Data Analysis

Business Intelligence

✅ Conclusion

The S&P 500 Stock Market Analysis Dashboard transforms a large historical stock dataset into an interactive financial analytics solution using Power BI.

The project combines company information with daily stock-market data and provides multiple analytical views, including S&P 500 Overview, Company Stock Analysis, Sector Analysis, and 25-Year Market Analysis.

It demonstrates how Power BI can be used to turn large financial datasets into meaningful visual insights for exploring company performance, sector composition, trading activity, and long-term market trends.

👨‍💻 Project

S&P 500 Stock Market Analysis Dashboard

Built with: Power BI | DAX | Power Query | Data Analytics
