# ETL_Top10Bank_Analysis
ETL on Top 10 Banks
# 🏦 ETL Bank Data Analysis: World's Top 10 Banks
## Author : Suaysh Nagar
## 📌 Introduction
This project presents a comprehensive ETL and analytics pipeline to examine the market capitalization of the world's top 10 banks. Using PySpark, Pandas, and cloud-native tools, it extracts, transforms, and visualizes financial data to uncover strategic insights into global banking dominance, currency conversions, and performance tiers.

## 🎯 Objective
- Identify the top 10 banks by market capitalization.
- Convert market cap values across multiple currencies (USD, GBP, EUR, INR).
- Perform exploratory and comparative analysis to reveal market concentration, dominance, and growth gaps.
- Store cleansed and enriched data in AWS S3 and SQLite for scalable querying.

## 🧰 Technical Stack
| Layer        | Tools & Services                              |
|-------------|------------------------------------------------|
| Cloud        | AWS EC2, AWS S3, Google Drive                 |
| ETL Engine   | PySpark, Pandas                               |
| Data Storage | CSV, SQLite3                                  |
| Visualization| Matplotlib, Seaborn                           |
| Logging      | Custom Python logging function                |
| Data Source  | Wikipedia (Archived September 2023)           |

## 🔄 ETL Pipeline Overview
- **Data Extraction**: Scrapes bank rankings and market cap from Wikipedia.
- **Currency Conversion**: Applies exchange rates from CSV to compute EUR, GBP, INR equivalents.
- **Data Cleaning**: Handles missing values, outliers (e.g., JPMorgan Chase), and schema fixes.
- **Storage**: Saves cleansed data to AWS S3 and Google Drive.
- **Querying**: Loads enriched data into SQLite3 for advanced querying and dashboarding.

## 📊 Key Analytical Modules
- **Market Cap Distribution**: Violin plots, quartile segmentation, and swarm plots.
- **Comparative Size Analysis**: Size vs average and top bank ratios.
- **Market Growth Gaps**: Absolute and percentage drop-offs between ranked banks.
- **Dominance Scoring**: Classifies banks into High, Moderate, and Low dominance tiers.
- **Segment-Wise Analysis**: Combines market cap quantiles with dominance and share metrics.

## 📈 Performance Dashboard Highlights
| Segment         | Avg Dominance | Market Share (%) | Bank Count |
|----------------|---------------|------------------|------------|
| Q1: Small Cap   | 0.66          | 21.97%           | 3          |
| Q2: Lower Mid   | 0.52          | 16.04%           | 2          |
| Q3: Upper Mid   | 0.36          | 27.01%           | 3          |
| Q4: Large Cap   | 0.23          | 34.98%           | 2          |

## 🧠 Strategic Conclusion
- **JPMorgan Chase** is the undisputed market leader with a cap of $432.92B—an outlier that skews all statistical averages.
- **Tiered Market Structure**: Tier 1 (JP Morgan) alone holds 22.8% of total market share; Tier 2 (Bank of America & ICBC) adds 22.4%; the remaining 7 banks share the rest.
- **Dominance vs Size Paradox**: Larger banks don’t always have higher dominance scores, suggesting strategic agility may lie in mid-tier players.
- **Growth Gaps**: A steep $201.4B (46.5%) drop between ranks 1 and 2, followed by a flatter curve—highlighting market asymmetry.

> 📁 _For full code, ETL scripts, and visual dashboards, refer to the code and Report

