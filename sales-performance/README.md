# Sales Performance Dashboard

An interactive Excel dashboard for analysing sales performance across time, region, product, customer type and sales channel.

## What it shows

**KPI cards**
- Total Revenue
- Total Orders
- Quantity Sold
- Average Order Value

**Charts**
- Revenue by Month (line)
- Revenue by Region (column)
- Revenue by Product Category (sorted column)
- Revenue by Sales Channel (donut)
- Top 5 Products by Revenue (bar)

## Filters

Dropdowns on the left of the Dashboard sheet: Quarter, Month, Region, Product Category, Customer Type, Sales Channel, plus From and To dates. Set a dropdown to "All" to clear it. All KPIs and charts update when a filter changes.

## Workbook structure

| Sheet | Purpose |
|---|---|
| Dashboard | KPI cards, charts and filters |
| Summary | Calculation tables that feed the dashboard |
| Data | Source data (2,000 orders, Jan to Dec 2026) plus helper columns |

## Data

- Source: [where the data came from, e.g. "Sample dataset from the tutorial linked below"]
- Columns: Order ID, Date, Region, Sales Channel, Customer Type, Product Category, Product, Salesperson, Quantity, Unit Price, Discount, Revenue
- Cleaning: about 1,200 dates were stored as text and were converted to real dates (month/day/year).
- Currency is not specified in the source data, so no currency symbol is shown.

## How it works

Each row in the Data sheet has an Include flag (1 or 0) based on the current filter selections. The Summary sheet uses SUMIFS and COUNTIFS on that flag, and the charts read from the Summary sheet. There are no pivot tables or macros.

## Inspiration

Based on a YouTube tutorial: [https://youtu.be/8fPLeLgO7Lg?si=M9wUvAukqlRSQU9W]

## Author

[Akhila Nare], [11/2026]