# 📊 Power BI Sales Performance Dashboard

Interactive 2-page Power BI report on sales performance, profitability, shipping and product returns, built on a two-table model (**Orders**, **Returns**) with DAX measures.

> **Status:** report published (`report/ProjetBI.pbix`). *(to complete: screenshots in `docs/screenshots/`, DAX formulas in `docs/dax_measures.md`)*

<!-- ![Page 1: overview](docs/screenshots/page1.png) -->
<!-- ![Page 2: analysis](docs/screenshots/page2.png) -->

## 🎯 Business questions answered
- How do sales, profit, units, orders and customers evolve by year, month, market and country?
- Which products are the most profitable, and which are returned the most?
- How do shipping cost and shipping delay relate to profit by category?
- What share of orders is discounted, and how large is the share of returned sales in Europe?

## 🖼️ Report content
**Page 1: overview.** KPI cards (total sales, total profit, total orders, total units sold, customers, average shipping cost); slicers (country, state, city, region, year, month, category, sub-category); Top 10 profit products and Top 10 returned products; donut, bar, column and line charts; filled map by country; gauge of the Europe share of returned sales.

**Page 2: analysis.** Sales by month and category (column chart); sales / net profit / shipping cost by category (scatter); share of discounted orders (pie); area and column charts.

## 📐 Data model and DAX
- **Tables**: `Orders` (order lines, enriched with `Ship Days`, `Profit Net`, `Sales avec Discount`, `Order Year`, `Order Month`, country code) and `Returns` (returned orders, region), related on the order identifier. Data preparation in Power Query. *(to complete: row count of each table and the Power Query steps)*
- **Measures used in the report**: `Total Sales`, `Total Units Sold`, `Total Orders`, `Customers`, `Total profit`, `Average Ship Coast`, `Orders with Discount`, `Total return`, `Total sales Retun`, `Total sales Retun Europe`. Formulas and explanations: [`docs/dax_measures.md`](docs/dax_measures.md).

## 🗂️ Data
The report is built on the same **Orders / Returns** sales data as the companion R project ([sales-data-cleaning-r](https://github.com/marwen-benhajkacem/sales-data-cleaning-r), 51,290 order lines and 1,079 returned orders). *(to complete: exact dataset name, source URL and licence.)*

A `.pbix` file embeds its data model. Read [SECURITY.md](SECURITY.md) and tick each point before the repository is made public. The licence below covers the report and documentation only, not the underlying dataset.

## ▶️ Open the report
1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows).
2. Clone or download this repository and open `report/ProjetBI.pbix`.
3. If Power BI asks for credentials or a refresh, do not enter credentials from an employer or private account.

## 📁 Structure
```
report/ProjetBI.pbix    the report (model + 2 pages)
docs/                   screenshots and DAX measures
SECURITY.md             pre-publication checklist
```

## 🛠️ Tools
Power BI Desktop · Power Query · DAX

## 👤 Author
Marwen Ben Haj Kacem · Master's in Data Science, ISIMA
