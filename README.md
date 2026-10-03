# Macroeconomic Outlook Dashboard | Power BI

## Project Overview

This project presents an interactive **Macroeconomic Outlook Dashboard** developed in Microsoft Power BI to compare the economic performance of four major economies:

- USA
- China
- India
- Japan

The analysis covers annual macroeconomic data from **2015 to 2025** and is built from a dataset containing **56 key macroeconomic indicators**.

The objective of the project is to provide a clear executive-level view of current economic conditions, historical trends, and cross-country differences.

---

## Dashboard Preview

![Macroeconomic Outlook Dashboard](dashboard-preview.png)

---

## Key Features

### Country Snapshot

The dashboard provides individual snapshots for USA, China, India, and Japan using four headline indicators:

- Real GDP Growth
- Inflation
- Unemployment Rate
- GDP Per Capita Growth

The dashboard also compares the latest values with the previous year using directional indicators.

### Economic Growth

The growth section includes:

- Real Consumption Growth
- Labor Productivity Growth
- Private Investment Growth
- Real GDP Growth Trend (2015–2025)

### Inflation & Prices

The inflation section includes:

- Headline Inflation
- Core Inflation
- Services Inflation
- Inflation Trend (2015–2025)

### Labour Market

The labour-market section includes:

- Unemployment Rate
- Labor Force Participation Rate
- Real Wage Growth
- Unemployment Trend (2015–2025)

### Key Indicator Snapshot

The 2025 cross-country comparison includes:

- Real GDP Growth
- GDP Per Capita Growth
- Inflation
- Unemployment Rate
- Policy Rate
- Current Account / GDP
- Government Debt / GDP

---

## Dashboard Interactivity

The dashboard includes:

- Country slicer
- Period slicer
- Cross-country comparisons
- 2025 vs 2024 KPI comparisons
- Historical trend analysis from 2015–2025
- Dynamic KPI calculations
- Interactive filtering

Historical trend charts are designed to retain the full 2015–2025 time series while selected snapshot indicators provide the latest-period comparison.

---

## Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX
- Microsoft Excel
- Data Cleaning
- Data Transformation
- Data Modeling
- Data Visualization
- Macroeconomic Analysis

---

## Example DAX

```DAX
Real GDP Growth 2025 =
CALCULATE(
    AVERAGE('Master_Wide'[Real GDP Growth (%)]),
    REMOVEFILTERS('Master_Wide'[Year]),
    'Master_Wide'[Year] = 2025
)

Data Coverage
Countries: USA, China, India, Japan
Period: 2015–2025
Frequency: Annual
Indicators: 56 macroeconomic indicators
The dataset covers areas such as economic growth, inflation, labour markets, monetary conditions, fiscal conditions, external-sector indicators, financial conditions, and other macroeconomic variables.
Data Sources
The project uses macroeconomic data compiled from official and internationally recognized statistical sources where applicable, including national statistical agencies, central banks, the World Bank, IMF, FRED and other official economic databases.
Source availability varies by indicator and country.
Note: Some latest-year observations may be estimates or latest available values depending on the publication schedule of the original source.

Key Dashboard Insights
The dashboard highlights significant differences in economic conditions across the four economies.
India and China show relatively stronger real GDP growth in the latest snapshot, while the USA and Japan show more moderate growth.
Inflation, unemployment, policy rates, government debt and current-account positions also vary considerably across countries.
The historical charts provide additional context by showing how growth, inflation and labour-market conditions evolved between 2015 and 2025.
Project Objective
The project demonstrates the use of Power BI for:
- Economic data analysis
- Cross-country comparison
- KPI development
- DAX calculations
- Historical trend analysis
- Executive dashboard design
- Business and management reporting
Author
Rajnandini Bhosale
Data Analyst | Power BI | SQL | Excel | Data Visualization
