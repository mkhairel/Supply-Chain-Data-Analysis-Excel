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

## Result Analysis & Strategic Insights

### 📦 1. High-Risk Supply Chain Exposure in Skincare Portfolio
A deep-dive cross-tabulation analysis reveals critical supply chain vulnerabilities concentrated within the highest-revenue product category (Skincare):

*   **Over-Reliance on Low-Efficiency Vendor (Supplier 3):** Based on the order quantity distribution matrices, Skincare accounts for the maximum volume allocated to `Supplier 3` with **415 units**, significantly eclipsing *Haircare* (185 units) and *Cosmetics* (32 units). Given that `Supplier 3` possesses the longest operational bottleneck with an average **Lead Time of 20.13 days**, the business faces an acute risk of sudden **stockouts** if seasonal delays escalate.
*   **Quality Threat from High-Defect Vendor (Supplier 5):** The Skincare segment holds an aggressive exposure of **344 ordered units** with `Supplier 5`. Diagnostic tracking identifies `Supplier 5` as the worst-performing manufacturer in terms of quality control, logging the highest average **Defect Rate of 2.67**. This directly threatens net profit margins due to inflated product waste and returns.

### 📉 2. Cost Outlier Diagnostic: The Chennai Transit Hub
Granular mapping of shipping carrier frequencies successfully isolates the root cause behind **Chennai's** inflated operational cost overhead (**RM 12,435.01**):
*   Operational logs confirm an aggressive dependency on infrastructure shipping models, specifically **Rail networks (6 instances)**, alongside Road (5 instances) and Sea (5 instances). 
*   **Analytical Inference:** The heavy reliance on Rail cargo corridors introduces fixed premium distribution surcharges, which act as the primary driver behind Chennai's elevated financial expenditure compared to other regional hubs.

### 🛠️ Strategic Procurement & Operational Recommendations
To successfully close this Exploratory Data Analysis (EDA) phase, the following risk-mitigation directives are proposed to the executive management:
1.  **Volume Rebalancing:** Restructure procurement contracts by shifting approximately 150 ordered units of Skincare from `Supplier 3` to `Supplier 1`—leveraging the latter’s faster turnaround cycle (**14.78 days**) and tighter quality assurance baseline (**1.80 defect score**).
2.  **Strict Quality Containment:** Mandate the Quality Assurance (QA) team to execute rigorous batch inspections specifically on all incoming Skincare lots originating from `Supplier 5` prior to warehouse intake to arrest downstream financial losses.

## Acknowledgements
- Special thanks to **Harsh Singh** for making this supply chain dataset openly available on Kaggle for analytics and data modeling validation.

## Files
- Data_Cleaning_Log
- Data_Inspection_Log
- Supply_Chain_Dashboard

## Author
- Muhamad Khairel
