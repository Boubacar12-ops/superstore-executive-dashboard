# Superstore Executive Business Performance Dashboard

Independent portfolio project analyzing the Sample Superstore dataset (public Kaggle dataset).

## Business Problem
Management has sales data but no clear view of performance. They need to understand total sales, profitability, and which categories and regions drive results and which need attention. This is an independent portfolio project; I did not work for a real company.

## Tools Used
Excel, Power BI

## Data Cleaning
- Original file: 9,995 rows.
- Removed 17 duplicate rows, leaving 9,977 transactions.
- 17 rows are missing Ship Mode, Segment, and Country (51 blank cells total). These fields aren't used in any KPI.
- The dataset has no order ID, order date, or customer ID.

## Key Findings
- **Total Sales**: $2,296,195.59  |  **Total Profit**: $286,241.42  |  **Profit Margin**: 12.47%  |  **Total Transactions**: 9,977
- **Category**: Technology has the highest sales ($836,154) and profit ($145,455). Furniture has $741,306 in sales but only $18,422 in profit, a 2.5% margin, compared with 17% for Technology and Office Supplies.
- **Region**: West earns the most profit ($108,330). Central earns the least ($39,656), with an 8% margin versus 15% in West. 32% of Central transactions lose money, versus 10% in West.
- **Products**: Tables (−$17,725), Bookcases (−$3,473), and Supplies (−$1,189) lose money. Tables and Bookcases are both in Furniture.
- **Discounts**: Transactions with no discount earned $320,844 in profit. Transactions with discounts above 20% lost about $135,000 combined. This is an association only; the data cannot prove that discounts cause the losses.

## Limitations
The dataset has no order ID, date, or customer ID, so order counts, customer counts, monthly trends, and growth rate could not be calculated and are not included.

## Dashboard
See the screenshots in this repo. The Sub-Category chart is sorted by profit; the lowest-profit sub-categories (Tables, Bookcases, Supplies) are visible by scrolling within the visual in the full `.pbix` file.

## Recommendations
- Investigate Furniture pricing and costs, starting with Tables and Bookcases, which lose money despite strong sales.
- Review the discount policy, especially discounts above 20%, and test capping them on Furniture.
- Investigate the Central region's pricing, shipping costs, and product mix against West.
- Study West's operations to see what could be applied in other regions.
- Collect order dates and customer IDs in future data so trends, growth, and customer analysis become possible.

## Files
- `SampleSuperstore.csv` — cleaned data
- `Project_2_Executive_Business_Performance_Dashboard.pbix` — Power BI dashboard
- `Project_2__Executive_Business_Performance_Dashboard.docx` — full analyst report
- Screenshots — dashboard images
