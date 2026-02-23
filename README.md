## 1. Project Overview

This project presents an interactive financial dashboard analyzing sales performance and overall profitability for the year 2023. The purpose of this dashboard is to provide business stakeholders with clear, data-driven insights into revenue trends, profit generation, and operational performance.

The analysis focuses on evaluating financial outcomes across product categories, sales channels, customer segments, and sales representatives in order to identify key drivers of profitability and performance variation.

The dashboard is designed to address the following strategic business questions:

- How did revenue evolve throughout the year?
- Which product categories contribute the most to overall profit?
- Which sales representatives generate the strongest profitability impact?
- How is revenue distributed across business quarters?
- How do different customer types influence overall financial performance?

By combining executive-level KPIs with interactive visualizations, the dashboard enables dynamic exploration of performance metrics and supports informed, data-driven decision-making.

## 2. Data Source & Overview

The dataset used in this project was obtained from Kaggle and consists of structured transactional sales records for the year 2023. The dataset represents simulated sales activity and is intended for analytical and educational purposes.

Each row represents a single sales transaction and includes detailed attributes related to product pricing, customer segmentation, and sales performance.

Key variables included in the dataset are:

- Product_ID  
- Sale_Date  
- Sales_Rep  
- Region  
- Product_Category  
- Quantity_Sold  
- Unit_Cost  
- Unit_Price  
- Sales_Amount  
- Customer_Type  
- Sales_Channel  
- Discount  

To enhance analytical value and financial reporting accuracy, additional derived metrics were created during the data preparation stage:

- **Profit**  
- **Monthly aggregation** 
- **Quarterly aggregation** 

These enhancements enabled structured financial analysis and supported the development of time-based and profitability-driven insights within the dashboard.

## 3. Steps & Methodology

The project followed a structured analytical workflow to ensure reliable financial reporting and meaningful dashboard insights.

### Data Validation & Preparation

The dataset was first explored using Python to understand its structure and overall quality. Descriptive statistics were reviewed to examine value distributions and detect potential anomalies. 

The following validation checks were performed:

- Identification of missing values across all variables.
- Verification of duplicate records.
- Review of numerical ranges for pricing and quantity fields.

The dataset was found to be structurally consistent and suitable for analysis without requiring extensive data cleaning.

### Data Transformation

To enable financial and time-based analysis, additional calculated fields were created:

- **Profit**  
  Profit = (Unit_Price − Unit_Cost) × Quantity_Sold  

- **Monthly aggregation** derived from `Sale_Date`
- **Quarterly aggregation** derived from `Sale_Date`

These transformations allowed for profitability tracking and structured performance reporting at different time granularities.

### Analysis Approach

The analysis focused on identifying key performance drivers rather than simply presenting descriptive statistics. The dashboard was structured to:

- Highlight overall financial performance through executive KPIs.
- Examine revenue trends across time.
- Evaluate profitability contribution by product category.
- Assess performance differences across sales representatives and channels.
- Support comparative analysis through interactive filters.

### Tool Selection

- Python (Pandas) was used for data validation and feature engineering due to its flexibility in handling structured datasets. 
- Looker Studio was selected for dashboard development because it enables interactive visualization, real-time filtering, and stakeholder-friendly reporting.

### Design Decisions

The dashboard layout follows an executive reporting structure:

- High-level KPIs positioned at the top for immediate visibility.
- Time-series analysis to capture performance evolution.
- Profitability breakdown across key business dimensions.
- Interactive controls to allow dynamic exploration.

The design prioritizes clarity, business relevance, and ease of interpretation for non-technical stakeholders.

## 4. Dashboard Screenshot 
<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/969fea97-d436-4664-aa78-6165ab0f63d3" />

## 5. Live Dashboard

[View Interactive Dashboard](https://lookerstudio.google.com/reporting/c281fccf-0bd6-456b-b4f1-e1b01043a4a0)

## 6. Key Insights

The dashboard analysis reveals consistent financial performance throughout 2023. Revenue remains relatively stable across months and quarters, with no extreme volatility observed. This indicates operational stability and steady sales activity throughout the year.


Profitability analysis highlights a clear imbalance across product categories. Certain categories, particularly Furniture and Clothing, contribute a significantly larger share of total profit compared to others. suggesting that specific segments of the product portfolio drive a stronger financial impact than others.

Performance variation is also visible at both the sales representative and sales channel levels. While Online and Retail channels contribute comparably to total profit, representative-level distribution suggests measurable differences in profitability contribution. This points to potential optimization opportunities in performance management, training, or incentive alignment to improve overall sales efficiency.

Customer segmentation analysis shows a strong contribution from returning customers, indicating effective retention performance. This reinforces the importance of maintaining customer loyalty strategies, as returning customers represent a stable and valuable revenue stream.

Overall, the dashboard demonstrates that profitability is driven not only by sales volume but by category mix, representative performance, and channel efficiency. Sustainable growth will depend on optimizing these drivers rather than solely increasing total sales volume.

## 7. Assumptions & Limitations

The dataset represents structured transactional sales data for the year 2023 only. As a result, the analysis does not capture multi-year performance trends or long-term seasonality patterns.

Profit is calculated at the transaction level using unit-based pricing, assuming that recorded unit cost and unit price values are accurate and consistent.

The analysis does not incorporate external market variables such as inflation, competitor pricing, economic conditions, or promotional campaigns.

Seasonal insights are limited to observations within a single year of data and may not reflect recurring long-term patterns.
