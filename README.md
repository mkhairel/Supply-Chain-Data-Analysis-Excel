# Supply-Chain-Performance-Risk-Analysis

## Project Overview
This project aims to analyze operational patterns within a supply chain network using transactional logistics data. The goal is to evaluate product profitability, measure supplier efficiency, and identify hidden supply chain bottlenecks to help management optimize inventory and mitigate operational risks.

## Objective
- Analyze product revenue and cost performance
- Identify factors influencing supplier delivery delays
- Perform data quality checking and structural validation
- Build multi-axis Pivot Tables for business evaluation
- Detect high-risk supplier dependencies within the network
- Generate prescriptive strategies for supply chain optimization

## Dataset
- The dataset consists of 100 operational entries from a Fashion and Beauty startup, tracking the supply chain of Makeup products.
- **Attributes:** Features 25 supply chain-related attributes including product types, SKU codes, pricing, revenue, manufacturing costs, supplier lead times, shipping modes, and defect rates.
- **Data Source:** Sourced from Kaggle: [Supply Chain Analysis Dataset](https://kaggle.com) uploaded by **Harsh Singh**.

## Tools
- Microsoft Excel
- Pivot Tables & Pivot Charts
- Calculated Fields (Data Modeling)
- Data Validation & Filtering Utilities

## Project Workflow
- Data Understanding
- Data Cleaning & Standardization
- Data Inspection (Sanity Checking)
- Exploratory Data Analysis (EDA)
- Business Logic Validation
- Insights & Prescriptive Recommendations

## Exploratory Data Analysis (EDA)
- Product revenue vs. cost analysis
- Supplier lead time profiling
- Manufacturing defect rate analysis
- Operational cost distribution by geographic hub
- Supplier-to-product cross-tabulation matrix
- Shipping carrier frequency analysis

## Data Inspection (Sanity Checking)
- Structural constraint audit (Verified file schema and boundaries)
- Business rule validation using logical checks (Revenue vs. Costs)
- Outlier and typo detection using extreme values (MIN/MAX)
- Post-cleaning integrity check using Excel Status Bar counts

## Data Modeling & Formulas
- Calculated Fields for Net Profit (`=Revenue - Costs`)
- Text standardization using `=TRIM()` and `=PROPER()`
- Operational count summaries via `=COUNTA()` and `=COUNTBLANK()`
- Custom number formatting for Currency (RM) and decimals

## Key Insights
- Skincare department recorded the highest revenue contribution at RM 241,628.16
- Supplier 3 demonstrated the longest turnaround delay with an average lead time of 20.13 days
- Supplier 5 showed the highest vulnerability in product quality with an elevated defect rate
- Skincare portfolio heavily relies on Supplier 3, introducing a high-risk bottleneck for stockouts
- Chennai hub registered the highest operational cost outlier due to premium rail freight dependency

## Analytical Dashboard
Dashboard includes:
- Product Revenue & Net Profit Comparison Chart
- Supplier Lead Time & Defect Performance Chart
- Geographic Cost Distribution Bar Chart
- Shipping Carrier Frequency Line Chart
- Dynamic Interactive Slicers for Location and Product filtering

## Business Problem
- Supply chain inefficiencies, unexpected logistics delays, and high product defect rates can result in massive revenue losses, operational disruptions, and stockout penalties. This project aims to identify the root causes of inflated distribution costs and operational bottlenecks to support proactive risk planning.

## Project Impact
- The project provides supply chain decision-makers with a data-driven approach to monitor vendor performance, identify high-risk product-supplier dependencies, and support strategic procurement planning through structured data visualization.

## Acknowledgements
- Special thanks to **Harsh Singh** for making this supply chain dataset openly available on Kaggle for analytics and data modeling validation.

## Files
- Data_Cleaning_Log
- Data_Inspection_Log
- Supply_Chain_Dashboard

## Author
- Muhamad Khairel
