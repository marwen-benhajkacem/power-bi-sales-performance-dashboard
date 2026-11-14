# Power BI Sales Performance Dashboard

An interactive Power BI report for exploring sales performance, profitability, orders, customers, products, shipping, and product returns.

## Project overview

This repository contains the Power BI report (`.pbix`) and documentation for reviewing and publishing the project.

The report contains two pages and includes:

- KPI cards for total sales, total profit, total orders, total units sold, customers, and average shipping cost.
- Filters for country, month, year, city, state, region, category, and sub-category.
- Product analysis, including top profitable products and returned products.
- Sales analysis by category, market, and year.
- Shipping-duration and discount-related visuals.
- Return analysis, including a regional view.

## Repository structure

```text
power-bi-sales-performance-dashboard/
├── README.md
├── SECURITY.md
├── GUIDE_FR.md
├── .gitignore
└── report/
    └── ProjetBI.pbix
```

## Open the report

1. Install [Microsoft Power BI Desktop](https://powerbi.microsoft.com/desktop/).
2. Download or clone this repository.
3. Open `report/ProjetBI.pbix` in Power BI Desktop.
4. If Power BI requests credentials or a data-source refresh, do not enter credentials from an employer or another private account. First confirm the source and your permission to use it.

## Data and privacy

The PBIX file contains an embedded Power BI data model. The report layout references fields such as product name, customer count, city, state, country, region, orders, sales, profit, and returns.

The repository creator must verify the origin, redistribution rights, and contents of the embedded data before making this repository public. Do not publish the PBIX publicly if it contains customer-level, commercially confidential, licensed, or otherwise restricted records.

If the data is based on a public sample dataset, document the exact dataset name, original source URL, license, and any required attribution here before public release. Do not claim that the data is public or synthetic unless that has been verified.

See [SECURITY.md](SECURITY.md) for the pre-publication checklist.

## Tools

- Microsoft Power BI Desktop
- Power BI data model and report visuals

## Notes

This repository currently contains the `.pbix` report file. It does not include a separate source dataset, Power Query source files, or a data dictionary. Those should only be added if they are yours to redistribute and have been checked for sensitive information.
