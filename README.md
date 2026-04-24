# TheLook eCommerce Financial Performance Analysis

## Overview
Financial performance analysis of TheLook eCommerce dataset using Google BigQuery and Tableau.
Examines revenue growth, category-level profitability, and product margin risk across 
1,400+ products and 26 categories from 2019 to 2023.

## Tools
SQL, Google BigQuery, Tableau

## Dataset
TheLook eCommerce — Google BigQuery Public Dataset  
`bigquery-public-data.thelook_ecommerce`

## Business Questions
1. Which product categories generate the most revenue and profit, and what are their margins?
2. Are there products operating at dangerously low margins?
3. Is overall revenue growing or declining over time?

## Key Findings
- Blazers & Jackets produced the highest profit margin at 62.03% despite ranking 15th in revenue
- Outerwear & Coats led all categories in total revenue but carried only a 55.52% margin, below several lower-volume categories
- Jeans ranked second in revenue ($1.24M) but had only a 46.48% margin, the largest 
  margin-to-revenue gap of any top-5 category
- Clothing Sets had the lowest margin across all categories at 38.29%
- Monthly revenue grew from $161 in January 2019 to over $25,000 by early 2023, 
  consistent compounding growth with no significant decline periods

## Files
- `queries/category_margin_analysis.sql` — revenue, cost, profit, and margin by category
- `queries/low_margin_products.sql` — products with margin below 40% on completed orders
- `queries/revenue_trend.sql` — monthly revenue trend for completed orders

## Tableau Dashboard
https://public.tableau.com/app/profile/kayden.williams2622/viz/TheLookeCommerceFinancialPerformanceAnalysisDashboard/TheLookeCommerceFinancialPerformanceAnalysis

## Business Recommendations
1. Investigate Jeans pricing strategy — second highest revenue category but 
   margin is 15+ points below top performers like Blazers & Jackets
2. Prioritize Blazers & Jackets and Accessories in marketing spend — 
   highest margins mean every incremental sale contributes more to profit
3. Review Clothing Sets and Socks categories — margins below 40% with low 
   revenue volume make these the weakest performers on both dimensions
