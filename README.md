# Financial Performance Dashboard Using Power BI

An interactive Power BI report built on Microsoft's [Financial Sample](https://learn.microsoft.com/en-us/power-bi/create-reports/sample-financial-download) workbook (700 sales records, September 2013 – December 2014). It covers 5 countries, 6 products and 5 customer segments.

The report has 5 pages: Executive Summary, Sales Analysis, Profit Analysis, Discount Analysis and Business Insights. Each page has slicers for month, country, product, segment and discount band.

**Tools:** Power BI Desktop, Power Query, DAX, Excel

![Executive Summary](Executive%20Summary.png)

## Business questions

1. How is the business doing overall (sales, profit, units sold, margin)?
2. How do sales and profit change from month to month?
3. Which countries, products and customer segments bring in the most sales?
4. Which products are the most profitable, and which have the best margin?
5. How much is spent on discounts, and how do discounts affect profit?

## Key metrics

| Total Sales | Gross Sales | Total Profit | Profit Margin | Units Sold | Total Discounts |
| --- | --- | --- | --- | --- | --- |
| $118.73M | $127.93M | $16.89M | 14.23% | 1.13M | $9.21M |

## Key insights

- **Sales are evenly spread across countries.** The United States ($25.03M), Canada ($24.89M), France ($24.35M) and Germany ($23.51M) are close, and Mexico is last ($20.95M). France makes the most profit ($3.78M).
- **Paseo is the top product**, with $33.01M in sales (27.8%) and $4.8M in profit. **Amarilla** has the best margin (15.86%), and **Velo** has the lowest (12.64%).
- **Government** is the biggest segment, with $52.50M in sales (44%) and $11.39M in profit. Small Business is second with $42.43M.
- **Enterprise loses money.** It brings in $19.61M in sales but makes a loss of about $0.61M.
- **October** has the highest sales and profit, and December comes second.
- **Bigger discounts cut profit margins.** Sales with no discount make a 21.9% margin, low discounts 17.9%, medium 14.4% and high only 9.1%. High-discount sales are about the same size as low-discount sales, but make about half the profit.

> Note: the data covers September 2013 – December 2014, so September to December appear in both years and January to August only in 2014. This partly explains why the last months of the year look stronger in the monthly charts.

## Recommendations

1. Limit high discounts. They take $5.3M of the $9.2M discount budget but give the lowest margin.
2. Review Enterprise pricing and costs to make the segment profitable.
3. Keep investing in Paseo and the Government segment, the biggest sources of profit.
4. Push higher-margin products such as Amarilla and VTT.
5. Prepare stock and campaigns for the strong October–December period.

## Report pages

| Page | What it shows |
| --- | --- |
| Executive Summary | KPI cards, monthly sales trend, sales by country, segment and product |
| Sales Analysis | Monthly sales trend, sales by product, segment and country |
| Profit Analysis | Profit by country and product, monthly profit trend, profit margin by product, sales vs profit |
| Discount Analysis | Total discounts, sales by discount band, monthly discount trend, discounts by product and country, discount vs profit |
| Business Insights | Top country, product, month and segment, plus a summary of key findings |

| Sales Analysis | Profit Analysis |
| --- | --- |
| ![](Sales%20Analysis.png) | ![](Profit%20Analysis.png) |

| Discount Analysis | Business Insights |
| --- | --- |
| ![](Discount%20Analysis.png) | ![](Business%20Insights.png) |

## Project structure

```
├── Power Bi Dashboards.pbix    Power BI report (all 5 pages)
├── Financial Sample.xlsx       source data
├── Executive Summary.png       page screenshots
├── Sales Analysis.png
├── Profit Analysis.png
├── Discount Analysis.png
└── Business Insights.png
```

## How to open

1. Install [Power BI Desktop](https://www.microsoft.com/en-us/power-platform/products/power-bi/desktop) (free, Windows only).
2. Open `Power Bi Dashboards.pbix`.
3. If Power BI can't find the data, go to **Transform data → Data source settings** and point it to `Financial Sample.xlsx` in this folder, then click **Refresh**.
