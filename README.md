# Supermarket Sales Analysis Dashboard (V2)

An Excel-based data analysis project that evaluates overall sales performance, product category and outlet comparisons, the relationship between product visibility and sales, and the statistical distribution of sales for a grocery retail business.

## Repository Structure

    supermarket-sales-analysis-v2/
    │
    ├── README.md
    ├── analysis and dashboard.xlsx
    ├── dataset.xlsx
    └── brief.pdf

## Project Overview

The objective of this project is to turn a raw sales dataset into an interactive Excel dashboard that helps supermarket management understand which categories and outlets perform best, how sales vary across outlet types, and whether product visibility has any bearing on sales. The dashboard lets management answer these questions without going through the full dataset.

The dataset contains 8,523 item-outlet records across 16 product categories and 10 outlets. The analysis is structured around four business objectives.

## Business Objectives

### 1. Overall Sales Performance
- Calculate total sales revenue.
- Calculate the average sales value per record.
- Calculate the average visibility of products across the supermarket.

### 2. Product Category and Sales Comparison
- Measure the share of total sales contributed by the top four categories versus all remaining categories.
- Identify the highest and lowest selling product categories.
- Compare total sales across outlet types.

### 3. Outlet Performance and Sales Relationships
- Compare sales across outlets for Low Fat and Regular products.
- Examine the relationship between product visibility and sales.
- Compare category sales contributions across outlet types.

### 4. Statistical Analysis of Sales
- Calculate the average, median, minimum and maximum sales values.
- Measure the variation in sales across records.
- Identify records with unusually high or low sales.
- Compare average sales across categories, outlet types and outlet locations.

## Workbook Structure

| Sheet | Description |
|---|---|
| `dataset` | Raw data as an Excel Table, plus a cleaned Fat Content column |
| `obj_1` to `obj_4` | One sheet per objective, with the analysis tables, formulas and charts |
| `dashboard` | KPI cards and charts controlled by four dropdown filters |
| `insights` | Insights, recommendations, and limitations and biases |

## Tools & Technologies

- Microsoft Excel
- Formula-driven analysis (SUMIFS, COUNTIFS, AVERAGEIFS, INDEX/MATCH, CORREL, QUARTILE, SKEW)
- Native Excel charts
- Dropdown filters for dashboard interactivity
- Statistical analysis and business insight writing

## Key Findings & Recommendations

### Key Findings

- **Overall Performance:** Generated approximately ₹1.20 million in sales across 8,523 records, averaging ₹140.99 per record, with an average product visibility of 6.61%.
- **Category Concentration:** The top four categories (Fruits and Vegetables, Snack Foods, Household and Frozen Foods) generate 50.6% of total sales. Fruits and Vegetables is the highest at about ₹178K, while Seafood is the lowest at about ₹9K.
- **Outlet Types:** Supermarket Type1 contributes 65.5% of sales, but it has six outlets compared with one each for Type2 and Type3. Average sales per record are almost identical across outlet types (₹139.80 to ₹141.68), so the gap reflects outlet count, not stronger sales per record.
- **Grocery Stores:** The two Grocery Store outlets average about ₹76K in sales per outlet versus about ₹131K for Supermarket Type1, because they carry far fewer records.
- **Visibility vs Sales:** There is no meaningful relationship between visibility and sales (correlation of about -0.001), and average sales do not rise or fall steadily across visibility bands.
- **Statistical Pattern:** Sales are roughly symmetric (mean ₹140.99, median ₹143.01) and no record is an outlier under the 1.5 x IQR rule. Category drives average sales (₹126 to ₹149 per record) far more than outlet type or location, which differ by under ₹2.

### Recommendations

- **Protect Core Categories:** Prioritise availability and shelf space for the top four categories, which carry about half of all sales.
- **Review Weak Categories:** Examine pricing, promotion and range for the lowest-average categories such as Baking Goods and Health and Hygiene.
- **Investigate Grocery Stores:** Check range depth, stock availability and footfall at the two Grocery Store outlets before judging their performance.
- **Test Before Investing in Visibility:** Run a controlled shelf-placement test, since the data shows no link between visibility and sales.
- **Strengthen Data:** Add dates, units sold, cost and margin, and enforce validation on Fat Content and visibility at source.

*Note: The dataset has no dates, no stated currency and no cost data, and some outlet types consist of a single outlet. Sales are shown in ₹ as an assumption, trends over time cannot be analysed, outlet-type effects cannot be separated from individual outlet effects, and about 6% of visibility values are zero and likely missing. Fat Content labels were standardised (LF and low fat to Low Fat, reg to Regular), and the findings should be read as descriptive rather than causal.*

## Project Files

| File | Description |
|---|---|
| `analysis and dashboard.xlsx` | Excel workbook containing the analysis, interactive dashboard, and insights. |
| `dataset.xlsx` | Dataset used for the analysis. |
| `brief.pdf` | Document outlining the project requirements and business objectives. |

## Business Value

This project demonstrates how Excel-based analysis can turn raw grocery sales data into clear, decision-ready insights.

The dashboard enables management to view total sales, average sales and visibility, compare categories and outlets, and see how sales are distributed, all in one place and filterable by outlet type, location, size and fat content.

## Conclusion

The project brings key sales, outlet, visibility and distribution metrics into a single Excel dashboard. The findings show that sales concentrate in a few categories, that outlet-level differences come mainly from outlet and record counts rather than per-record performance, and that visibility does not explain sales in this data. Improving data capture would allow deeper analysis of trends and profitability in future work.
