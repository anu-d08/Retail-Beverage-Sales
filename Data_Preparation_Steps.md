Data_Preparation_Steps – Retail Beverage Sales Dashboard
1️.Raw Data Overview

Source: Raw_Beverage_Sample sheet within the main Excel workbook.

Contains six months (Jan–Jun) of retail transactions across multiple outlets.

Key columns include:
Transaction_ID, Product_ID, Store_ID, Date, Time, Category, Product, Store_Location, Sales_Amount, Quantity, and Order_Size.

2️.Cleaning & Transformation

Performed using Excel Power Query to ensure consistency and analytical readiness:

Removed duplicate rows and entries with missing Date, Category, or Sales_Amount.

Standardized date/time formats and extracted new fields:

Hour – for hourly sales trend analysis

Weekday – for weekly traffic distribution

Month – for trend comparison across periods

Converted all currency and quantity fields to numeric data types.

Ensured proper casing for categorical fields (e.g., “Coffee”, “Bakery”, “Smoothie”).

Created derived metrics:

Avg_Bill_Per_Customer = Total_Sales / Total_Customers

Avg_Orders_Per_Customer = Total_Orders / Total_Customers

3️.Data Aggregation

Grouped transactions by:

Hour → for identifying daily demand cycles

Store_Location → for comparing performance across regions

Category → for product-level contribution analysis

Aggregated KPIs:

Total_Sales, Total_Orders, Customer_Count, and Avg_Bill_Per_Customer.

4️.Validation & Consistency Checks

Verified that aggregate totals matched raw source sums (variance ≤ 0.01).

Checked for outliers in revenue and order quantity using percentile thresholds.

Cross-checked monthly and hourly totals to confirm logical consistency.

5️.Output & Integration

Final dataset exported as Cleaned_Retail_Beverage sheet within the dashboard workbook.

Structured for direct connection to the Excel dashboard visuals.

Dataset linked dynamically to KPI cards, slicers, and PivotCharts.


Tools Used

Microsoft Excel (Power Query): Data import, cleaning, and aggregation

PivotTables: Analytical summaries for trend and KPI visualization

Data Validation Tools: Duplicate detection and outlier control

Data Disclaimer

This dataset is a synthetic, anonymized sample created for portfolio demonstration purposes.
It does not represent real customer or store information.