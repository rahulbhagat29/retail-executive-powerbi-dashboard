📊 Retail Executive Revenue & Margin Performance Analysis
📌 Business Problem

A multi-category retail business experienced steady revenue growth between 2022 and 2024. However, leadership lacked visibility into whether growth was sustainable, margin-efficient, and evenly distributed across products, regions, and customer segments.

Without structured performance analysis, the company could not answer critical financial stability questions:

Is revenue growth translating into stable profit margins?
Are discounts eroding profitability at the sub-category level?
Is performance concentrated in specific regions or customer segments?
Are a small number of products or customers driving disproportionate revenue?

This analysis answers three critical executive questions:

Is growth healthy and margin-efficient?
Where are profitability risks emerging?
Is revenue diversified or concentrated?

🎯 Key Findings

Revenue Performance Stability: Revenue reached $6.55M with strong YoY growth, while maintaining a stable ~27.7% profit margin. Growth is not occurring at the expense of profitability.

Discount Impact Assessment: Higher discount clusters show slight margin compression but no severe erosion. Pricing strategy remains controlled at the sub-category level.

Category & Product Distribution: Revenue contribution is balanced across major categories, reducing over-dependence risk. However, bottom-performing products indicate potential pricing or positioning inefficiencies.

Customer & Segment Insights: The Consumer segment leads revenue generation with strong margin performance. Revenue concentration among top customers exists but does not indicate extreme dependency risk.

Regional Comparison: Regional revenue distribution remains relatively balanced, with no major structural margin weaknesses.

💼 Business Recommendations

Immediate Actions:

Review bottom-performing products for pricing optimization or product bundling strategies
Maintain disciplined discounting strategy to prevent gradual margin dilution
Monitor regional margin performance to detect early structural divergence
Strengthen performance tracking for high-value customer clusters

Strategic Direction:

Adopt margin monitoring as a primary KPI alongside revenue growth
Introduce rolling 12-month trend tracking for forward-looking stability assessment
Implement product-level profitability dashboards for monthly executive review
Shift performance reviews from revenue-only discussions to margin-adjusted analysis

🔍 Analytical Approach

Data Modeling (Power BI):

Built a star schema model separating fact and dimension tables
Established one-to-many relationships between Date, Product, Customer, and Sales tables
Marked Date table to enable time-intelligence calculations

Revenue & Margin Analysis (DAX):

Created Total Revenue and Total Profit measures
Calculated Profit Margin using safe DIVIDE logic
Built YoY and MoM growth measures using time intelligence
Implemented Top/Bottom ranking measures for product analysis

Risk & Concentration Analysis:

Analyzed discount vs margin relationship at sub-category level
Evaluated category-level revenue contribution
Measured customer-level revenue concentration
Compared regional revenue and margin performance

Visualization:

Designed executive-ready dashboard with three structured pages
Applied consistent layout hierarchy and KPI strip
Built drill-down category visuals for deeper analysis
Presented balanced mix of trend, comparison, and ranking visuals

📊 Data Overview

The analysis uses structured transactional data modeled into a star schema format.

Each row in the fact table represents a single transaction record.

Data Schema (Analysis Dataset):

| Column Name | Description                   |
| ----------- | ----------------------------- |
| Order_ID    | Unique transaction identifier |
| Order_Date  | Date of transaction           |
| Customer_ID | Unique customer identifier    |
| Product_ID  | Unique product identifier     |
| Quantity    | Units sold                    |
| Sales       | Revenue generated             |
| Cost        | Cost of goods sold            |
| Profit      | Calculated transaction profit |
| Discount    | Discount applied              |

Dimension Tables:

| Table Name   | Description                               |
| ------------ | ----------------------------------------- |
| dim_date     | Calendar hierarchy (Year, Quarter, Month) |
| dim_customer | Customer segment and regional attributes  |
| dim_product  | Category and sub-category classification  |

Time Period Covered: 2022–2024

🛠 Technical Stack

Power BI: Data modeling, dashboard development
DAX: Time intelligence, ranking, margin calculations
Excel: Source dataset preparation
Star Schema Modeling: Fact and dimension structuring

⚠️ Limitations

Analysis is based solely on transactional financial data.
No marketing spend data was included to calculate ROI impact.
Customer lifetime value (CLV) was not calculated due to limited historical depth.
External economic or seasonality variables were not incorporated.

🔮 Future Enhancements

Add Rolling 12-Month revenue and margin tracking
Implement drill-through product detail page
Incorporate customer lifetime value modeling
Build decomposition tree for dynamic revenue breakdown
Automate data refresh pipeline for monthly executive reporting
