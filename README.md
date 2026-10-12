# Electric Vehicle Sales Analysis | Excel Dashboard

## Project Overview

This project analyzes electric vehicle (EV) sales data using Microsoft Excel. It explores sales trends, vehicle types, brands, models, customer demographics, payment methods, financing status, delivery timelines, and customer ratings.

The objective is to understand how sales are distributed across the available business dimensions and identify useful opportunities for improving sales reporting and customer experience.

## Business Problem

EV businesses need to understand which vehicles contribute most to sales, how sales activity changes over time, and whether the customer experience remains consistent across brands, locations, and sales channels.

This project explores the following questions:

* How does recorded sales value change over time?
* Which vehicle types account for the highest number of sales records?
* How do brands and models compare in recorded sales value?
* How are sales distributed between online and dealer channels?
* Which states contribute the most sales records?
* What are the average selling price, delivery time, and customer rating?
* How are payment methods and loan status distributed?

## Dataset Overview

* **Total records:** 15,800
* **Total columns:** 22
* **Reporting period:** January 2022 to July 2025
* **Tool:** Microsoft Excel

The dataset includes Sale ID, Sale Date, Customer Name, Gender, Age, State, City, Dealer Name, Brand, Model, Vehicle Type, Battery Capacity, Range, Quantity, Unit Price, Discount, Total Sale, Payment Mode, Loan Status, Delivery Days, Sales Channel, and Customer Rating.

## Tools & Techniques

* Microsoft Excel
* PivotTables and PivotCharts
* KPI calculations
* Sales trend analysis
* Category-wise comparisons
* Customer and geographic segmentation
* Dashboard-based reporting

## Dashboard Preview
<img width="979" height="743" alt="Screenshot 2026-10-12 091331" src="https://github.com/user-attachments/assets/51cd5480-441e-4cf7-88ea-e8b33fe2834a" />
<img width="973" height="178" alt="Screenshot 2026-10-12 091341" src="https://github.com/user-attachments/assets/29e0e3f6-1e85-47eb-aa56-a819947ad61f" />




## Key Performance Indicators

| KPI                        |         Result |
| -------------------------- | -------------: |
| Total Sales Records        |         15,800 |
| Total Recorded Sales Value | 28,358,167,382 |
| Average Selling Price      |   1,794,820.72 |
| Total Discount Recorded    |    789,054,107 |
| Average Delivery Time      |      7.98 days |
| Average Customer Rating    |       3.99 / 5 |
| Online Sales Records       |          7,931 |
| Dealer Sales Records       |          7,869 |



### KPI Definitions

**Total Recorded Sales Value:** Sum of the `Total_Sale` field.

**Average Selling Price:** Average of the `Unit_Price` field.

**Average Delivery Time:** Average of `Delivery_Days`.

**Average Customer Rating:** Average of the recorded `Customer_Rating` values.

These metrics summarize the available dataset and should be interpreted according to the business definitions used in the source workbook.

## Chart-by-Chart Analysis

### 1. Total Sales by EV Model

**Chart type:** Bar chart.

**Purpose:** To compare recorded sales value across individual EV models.

**How to read it:** Each bar represents a vehicle model, and its length represents the corresponding sales value. Longer bars indicate higher recorded sales value.

**Business interpretation:** The chart helps identify models contributing a larger share of the recorded sales value.

**Recommended action:** Compare model-level sales value with units sold, average selling price, discounts, and customer ratings to understand whether higher value comes from sales volume or pricing.

### 2. Sales by Year

**Chart type:** Line chart.

**Purpose:** To compare recorded sales value across calendar years.

**How to read it:** Each point represents the total recorded sales value for a year.

**Business interpretation:** The workbook records approximately 8.02 billion in 2022, 7.96 billion in 2023, and 7.96 billion in 2024. The recorded 2025 value is approximately 4.41 billion, but the dataset only runs through July 2025.

**Recommended action:** Avoid comparing the partial 2025 total directly with full-year totals. Use a year-to-date comparison for the same months to evaluate trends more fairly.

### 3. Sales Value by Brand

**Chart type:** Bar chart.

**Purpose:** To compare recorded sales value across EV brands.

**How to read it:** Each bar represents the sales value associated with a brand.

**Business interpretation:** The recorded sales values are relatively close across the five brands, with MG contributing approximately 5.84 billion and Tata approximately 5.54 billion.

**Recommended action:** Compare brand-level sales value with units sold, average selling price, model mix, and customer ratings before making product or marketing decisions.

### 4. Monthly Sales Trend

**Chart type:** Line chart.

**Purpose:** To monitor recorded sales value across months.

**How to read it:** Each point represents the total sales value associated with a month.

**Business interpretation:** The recorded monthly values vary, with January, March, and May among the higher-value months in the workbook's monthly summary.

**Recommended action:** Investigate monthly variations alongside units sold, discounts, and vehicle mix. If the chart is intended to show seasonality, use a consistent month-by-month comparison across multiple years.

**Chart improvement:** Exclude the Grand Total row from the chart source. The monthly chart should contain only January through December, not an additional total category.

### 5. Vehicle Type Distribution

**Chart type:** Category comparison chart.

**Purpose:** To compare sales record counts across Sedan, SUV, and Hatchback vehicles.

**How to read it:** Each category shows the number of records associated with a vehicle type.

**Business interpretation:** Sedan accounts for 5,365 records, SUV for 5,273, and Hatchback for 5,162. The distribution is relatively balanced.

**Recommended action:** Compare vehicle type with sales value, discount, delivery time, and customer ratings to identify differences in customer experience and sales contribution.

### 6. Sales Channel Distribution

**Chart type:** Doughnut or pie chart.

**Purpose:** To compare sales records between Online and Dealer channels.

**How to read it:** Each segment represents the proportion of records associated with a sales channel.

**Business interpretation:** Online accounts for 7,931 records, approximately 50.20%, while Dealer accounts for 7,869 records, approximately 49.80%.

**Recommended action:** Compare channel-level sales value, average selling price, discounts, and customer ratings to understand whether the channels differ in business outcomes.

### 7. Sales by State and Brand

**Chart type:** Cross-tabulation or heatmap.

**Purpose:** To examine how recorded customer sales are distributed across states and brands.

**How to read it:** Rows represent states, columns represent brands, and the values represent the number of customer records.

**Business interpretation:** This view allows state-level brand preferences and differences in record volume to be explored.

**Recommended action:** Compare the distribution with sales value and vehicle model mix before deciding where marketing or dealer resources should be focused.

### 8. Payment Method Distribution

**Chart type:** Column or doughnut chart.

**Purpose:** To summarize the distribution of records across payment methods.

**How to read it:** Each category represents a payment method and its corresponding record count.

**Business interpretation:** The chart provides a descriptive view of how customers pay for recorded vehicle purchases.

**Recommended action:** Compare payment methods with average selling price and loan status, while confirming that each field is consistently recorded.

### 9. Loan Status Distribution

**Chart type:** Column or doughnut chart.

**Purpose:** To understand how records are distributed by loan status.

**How to read it:** Each category represents the recorded loan status.

**Business interpretation:** The workbook contains 7,869 records marked Yes and 7,931 marked No.

**Recommended action:** Compare loan status with vehicle model, sales channel, and delivery time to investigate any operational differences. Loan status alone does not indicate credit approval quality or customer risk.

### 10. Customer Rating Analysis

**Chart type:** Rating distribution or average rating chart.

**Purpose:** To summarize customer feedback recorded in the dataset.

**How to read it:** A rating distribution shows the number of customers giving each score, while an average-rating chart summarizes the mean score.

**Business interpretation:** The overall average customer rating is approximately 3.99 out of 5.

**Recommended action:** Compare ratings across brands, vehicle types, dealers, and delivery times to identify where customer experience may differ.

### 11. Delivery Time Analysis

**Chart type:** KPI card or comparative chart.

**Purpose:** To understand the time taken to deliver vehicles.

**How to read it:** The average delivery time is approximately 7.98 days. Grouped charts can compare this metric across brands, models, states, or channels.

**Business interpretation:** The average provides a high-level view, but it does not show whether a small number of delayed deliveries are affecting the overall result.

**Recommended action:** Add median delivery time and the percentage of deliveries completed within a business-defined target to understand delivery performance more fully.

## Key Business Observations

The dataset contains 15,800 sales records and a total recorded sales value of 28,358,167,382.

The annual sales summaries show broadly similar recorded values for 2022, 2023, and 2024. The 2025 total is based on data through July, so it is not directly comparable with complete calendar years.

Sales records are distributed relatively evenly across Sedan, SUV, and Hatchback categories. Online and Dealer channels also account for similar proportions of records.

MG has the highest recorded brand-level sales value in the available summary, while Kona Electric has the highest recorded model-level sales value in the model comparison.

The average delivery time is approximately 7.98 days, and the average customer rating is approximately 3.99 out of 5. Further segmentation would help determine whether these indicators vary meaningfully across brands, models, or locations.

## Recommendations

1. Compare year-to-date sales for consistent periods before evaluating annual growth.
2. Analyze sales value alongside quantity and average selling price.
3. Review brand and model performance using discounts and customer ratings.
4. Compare online and dealer channels on sales value, not only record counts.
5. Investigate delivery-time differences across dealers and vehicle models.
6. Examine lower customer ratings alongside delivery time and vehicle type.
7. Validate the meaning and currency of financial fields before presenting commercial conclusions.

## Limitations

The analysis is based on the fields and values available in the workbook. The currency is not explicitly identified in the available columns.

The dataset contains dates only through July 2025, so the 2025 annual figure is incomplete. Record counts should not automatically be described as unique customers or completed vehicle deliveries without validating the underlying business definitions.

The observed differences are descriptive and do not establish the causes of sales performance or customer satisfaction.

## Conclusion

This project demonstrates how Microsoft Excel can be used to analyze EV sales records, compare brands and vehicle models, monitor sales trends, and summarize customer and operational indicators.

By combining financial metrics with product, channel, geographic, and customer-experience dimensions, the analysis provides a foundation for further investigation and more informed business decisions.

## Author

**Vansh Kumar**
Aspiring Data Analyst

**Skills:** Excel, data analysis, KPI reporting, business insights, and data visualization.
