# Arunya-Retail-Sales-Analysis

## 1. Project Overview

This project analyzes retail secondary-sales data for June and July 2026 for **Aarunya Consumer Products**, a fictional company name used to anonymize the original assignment context.

The project demonstrates a business analytics workflow involving data cleaning, sales performance analysis, KPI reporting, anomaly identification, and business recommendations.

### Business Objectives

- Clean and standardize distributor, outlet, SKU, and transaction data.
- Compare June and July sales performance and month-on-month (MoM) changes.
- Analyze distributor sales, product performance, and active outlet coverage.
- Identify anomalies and recommend further investigation.
- Propose a repeatable approach for consolidating multi-source sales reports.

## 2. Tools Used

| Tool | Purpose |
|---|---|
| Microsoft Excel | Data analysis, pivot tables, charts, dashboard development, and KPI reporting |
| Power Query | Data cleaning, transformation, and standardization |
| Microsoft Word | Documenting business anomalies and case-study responses |

## 3. Data-Cleaning Methodology

The source dataset contained 320 rows across five distributors, with inconsistent naming, duplicate records, mixed date formats, and missing values.

The cleaning process included:

- **Distributor standardization:** Standardized inconsistent distributor names referring to the same distributor.
- **SKU standardization:** Normalized inconsistent product names, including variations in sesame oil product names.
- **Duplicate handling:** Reviewed and removed duplicate records, including duplicates identified after name standardization.
- **Missing-value treatment:** Flagged records with missing `Qty_Sold` and `Sales_Value` as incomplete or unbilled transactions and excluded them from sales-sum calculations.
- **Date transformation:** Converted dates to a consistent format for month-based analysis.
- **Cleaning documentation:** Maintained a cleaning log documenting identified issues, transformations, and the rationale behind decisions.

Refer to the **Cleaning Log** worksheet for the specific transformation steps.

## 4. Sales Analysis, KPI Reporting, Charts and Dashboard

The project includes an Excel-based sales analysis dashboard built using pivot tables and charts to present key performance indicators (KPIs), compare monthly performance, and identify business trends.

The analysis covers:

- **Sales by Distributor:** Compares total sales value across distributors for June and July.
- **Sales by Category and SKU:** Analyzes product and category-level sales performance.
- **Active Outlet Analysis:** Tracks the number of active outlets under each distributor.
- **Month-on-Month (MoM) Analysis:** Highlights changes in sales performance between June and July.
- **Top and Bottom 3 SKUs:** Identifies the highest- and lowest-performing SKUs by sales value.
- **Charts and Data Visualization:** Visualizes sales trends and performance comparisons for easier interpretation.
- **Excel Dashboard:** Brings key sales metrics and visual summaries together to support quick business review and decision-making.
- **Anomaly Identification:** Highlights significant sales declines that require further investigation.

## 5. Key Findings

### 5.1 Cold Pressed Coconut Oil 500ml

Sales declined from **₹108,242 in June to ₹81,652 in July**, representing an approximate **24.5% decrease**.

**Recommended investigation:**
- Analyze the decline by distributor and outlet.
- Check product availability and potential stock-outs.
- Review outlet activity and changes in demand.
- Investigate possible pricing or promotional changes.

### 5.2 Trichy Central Distributors

Sales declined from approximately **₹2.01 lakh in June to ₹1.25 lakh in July**, a decrease of approximately **37.8%**.

Additional observations:

- Active outlets decreased from **13 to 9**, a decline of approximately **31%**.
- Quantity sold decreased by approximately **32%**.

The simultaneous decline in sales, quantity, and active outlets suggests that reduced outlet activity may be contributing to the sales drop. However, the available data does not establish the root cause.

**Recommended investigation:**
- Validate the figures against the RTA/DMS platform.
- Identify inactive outlets and underperforming SKUs.
- Review stock availability, order frequency, and sales coverage.
- Consult the field sales team to understand operational issues.

## 6. Proposed Reporting Automation Approach

To consolidate quick-commerce sales, offline secondary sales, and online marketplace or store data into a repeatable weekly report, the proposed approach is:

1. **Source collection:** Gather exports from each sales channel through a consistent weekly process.
2. **Data standardization:** Align column names, date formats, SKU names, channel labels, and sales-value formats.
3. **Power Query transformations:** Clean and append datasets into a consistent structure.
4. **Mapping tables:** Maintain reference tables for distributor names, SKUs, and sales channels.
5. **Data validation:** Check missing values, duplicate records, date ranges, and totals against source reports.
6. **Reporting refresh:** Update pivot tables or, where available, a Power BI report using the consolidated dataset.
7. **Exception tracking:** Maintain a data-quality log for unresolved issues and transformation changes.

*This is a proposed reporting approach; a complete automated multi-source pipeline was not implemented as part of this project.*

## 7. Recommendations

### Sales Performance

- Investigate the 24.5% SKU sales decline at distributor and outlet levels.
- Review the decline in Trichy Central Distributors' sales and active outlet coverage.
- Cross-check sales figures against source systems to rule out data-entry or reporting errors.
- Consult the field sales team about stock-outs, missed visits, order frequency, returns, and demand changes.

### Reporting and Data Quality

- Keep raw source data separate from cleaned and summarized datasets.
- Maintain standardized naming conventions and mapping tables.
- Use documented Power Query steps to reduce repetitive manual work.
- Add validation checks for duplicates, missing values, and unexpected changes in totals.
- Document assumptions and unresolved data-quality issues.

### Outlet-Servicing Decisions

Outlet servicing decisions should not be based on sales value alone.

Before recommending that an outlet should no longer be serviced:

- Clarify the business objective, such as low sales, low profitability, high servicing cost, or inactivity.
- Review outlet-level sales, quantity, activity, and historical trends.
- Collect additional profitability or servicing-cost data if required.
- Discuss the findings with the relevant stakeholder or field sales team before making a final decision.


## 8. Key Learnings

- Data standardization is essential for accurate distributor and SKU comparisons.
- Duplicate and incomplete records require transparent and documented treatment.
- Sales value becomes more informative when analyzed alongside quantity sold and active outlet counts.
- An anomaly is a starting point for investigation, not proof of its cause.
- Mapping tables and repeatable Power Query transformations can improve reporting consistency.
- Business decisions require clear objectives and appropriate operational and financial information.

## 9. Data-Sharing Disclaimer

**Aarunya Consumer Products is a fictional name used for anonymization.**

This project is based on an assignment dataset. 
