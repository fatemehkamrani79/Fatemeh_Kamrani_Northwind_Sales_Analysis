# Northwind Sales Analysis in Excel

I completed this project as Excel Exercise 04 in the Data Analyst Training Program at Tose'e Institute, taught by Dr. Majid Eyvazian.

The assignment was to combine the Northwind tables with XLOOKUP, calculate net sales, and answer a set of sales questions with PivotTables and PivotCharts. After completing the required tasks, I added two dashboard pages, validation checks, and project documentation to make the workbook easier to review.

## Assignment Information

- **Institute:** Tose'e Institute
- **Instructor:** Dr. Majid Eyvazian
- **Course:** Data Analyst Training Program
- **Exercise:** Excel Exercise 04

The original assignment is available in the [`docs`](docs/Excel_Exercise_04_Assignment.pdf) folder.

## Original Assignment

The main tasks were:

- Combine the Orders and Order Details tables using `OrderID` and `XLOOKUP`
- Calculate net sales from unit price, quantity, and discount
- Add category names to the Products and Order Details data
- Analyze quarterly and monthly sales trends
- Find the top products, categories, and customers
- Compare category sales across quarters
- Review the monthly sales trend for each category

## My Work

I kept the original Northwind tables in separate raw-data sheets and created new tables for the analysis. Customer, product, category, date, month, quarter, and net sales fields were added before building the PivotTables and charts.

Net sales were calculated as:

`UnitPrice × Quantity × (1 - Discount)`

The finished workbook includes an executive dashboard, a separate category analysis page, data-quality checks, and a short documentation sheet.

## Dashboard

### Executive Dashboard - KPIs, Trends, Products, and Categories

The first part of the dashboard includes the main KPIs, monthly and quarterly sales trends, top products, and category results.

![Executive dashboard KPIs trends products and categories](images/executive_dashboard_01.png)

### Executive Dashboard - Customers and Key Insights

The second part shows the leading customers by net sales and a short summary of the main findings.

![Executive dashboard customer results and key insights](images/executive_dashboard_02.png)

### Category Analysis

This page compares quarterly category sales with a heatmap. The monthly trend chart can be filtered by category using the slicer.

![Category sales analysis](images/category_analysis.png)

## Key Results

- Total net sales were **$1.27M** across **830 orders**.
- Q1 1998 was the strongest complete quarter, with **$298K** in net sales.
- April 1998 was the strongest complete month, with **$124K** in net sales.
- Côte de Blaye generated **$141K**, which was 76% more than the second-ranked product.
- Beverages and Dairy Products together generated 40% of total net sales.
- The top three customers generated 25% of total net sales.

## Workbook Structure

| Sheet | Purpose |
|---|---|
| `Raw_Categories` | Original category data |
| `Raw_Order_Details` | Original order-detail data |
| `Raw_Orders` | Original order data |
| `Raw_Products` | Original product data |
| `Sales_Data` | Prepared sales analysis table |
| `Products_Data` | Prepared product table |
| `Analysis_Support` | PivotTables and dashboard calculations |
| `Executive_Dashboard` | Main sales dashboard |
| `Category_Analysis` | Category heatmap and monthly trend |
| `Data_Validation` | Data-quality checks and correction log |
| `Documentation` | Project notes and methodology |

## Excel Features Used

- Excel Tables
- XLOOKUP
- PivotTables and PivotCharts
- Slicers
- Conditional Formatting
- Data validation checks
- Internal navigation links

## Data Quality Checks

Before finalizing the workbook, I checked row counts, duplicate records, missing values, lookup results, changes to the source data, sales totals, and the calculations used by the dashboards. All **22 validation checks passed**, with no items left for review.

One invalid `UnitPrice` value was found for ProductID 42. The original value remains in the raw-data sheet, while the corrected value of **$14.00** is used in the analysis table and recorded in the validation log.

## How to Use the Workbook

1. Download `Fatemeh_Kamrani_Northwind_Sales_Analysis.xlsx`.
2. Open it in Microsoft Excel desktop.
3. Start with the `Executive_Dashboard` sheet.
4. Open `Category_Analysis` to review category performance.
5. Use the slicer to change the category shown in the monthly trend chart.

Excel desktop is recommended because the workbook uses PivotTables, PivotCharts, a slicer, and internal navigation.

## Data Notes

- The analysis covers July 4, 1996 through May 6, 1998.
- July 1996 and May 1998 are partial months.
- Q2 1998 is a partial quarter.
- Product cost, profit, and sales targets are not included in the dataset.

## Project Files

```text
Fatemeh_Kamrani_Northwind_Sales_Analysis/
├── README.md
├── Fatemeh_Kamrani_Northwind_Sales_Analysis.xlsx
├── docs/
│   └── Excel_Exercise_04_Assignment.pdf
└── images/
    ├── executive_dashboard_01.png
    ├── executive_dashboard_02.png
    └── category_analysis.png
```

## Author

**Fatemeh Kamrani**  
[GitHub Profile](https://github.com/fatemehkamrani79)

