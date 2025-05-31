# AtliQ Hardware Financial Analytics – Deep Analysis Report

## 1. Project Overview

AtliQ Hardware is a growing consumer electronics company. Previously, the company relied on Excel for reporting, which resulted in slow, fragmented, and error-prone financial analysis. This project delivered a **Power BI dashboard solution**, enabling real-time, accurate, and actionable financial insights for management.

---

## 2. Business Context & Problem Statement

- **Business Model:** AtliQ manufactures and distributes hardware via B2B channels and direct retail.  
  Financial flow: Manufacturing → Warehouse → Stores/Online → Customers.

- **Challenges:**
  - Reliance on Excel led to data silos, slow reporting, and manual errors.
  - Increasing business complexity required dynamic analysis.
  - Leadership lacked timely visibility into financial performance.

---

## 3. Data Infrastructure & Preparation

- **Sources Integrated:** Sales, customers, products, regions, targets.
- **Power Query ETL:**
    - Data cleaning: removed duplicates, and standardized formats.
    - Merged multiple data sources.
    - Applied **fiscal year logic**: AtliQ’s FY is September–August.
- **Data Model:**
    - **Star schema:** Central fact table (sales), dimension tables (date, product, customer, market).
    - Custom **Date Dimension** for time intelligence (YTD, YOY, fiscal period).

**![Insert Data Model Screenshot Here](../images/data_model.png)**

---

## 4. Key Financial Terminologies & Calculations

| Term         | Definition/Logic                                       | Project Example              |
|--------------|--------------------------------------------------------|------------------------------|
| Gross Price  | Product price before discounts/deductions              | Used as base price           |
| Net Price    | Gross Price minus discounts (pre/post invoice)         | Final selling price          |
| Gross Sales  | Gross Price × Quantity                                 | Initial sales total          |
| Net Sales    | Gross Sales after all deductions/discounts             | Revenue post-discounts       |
| COGS         | Direct costs: manufacturing, freight, taxes, packaging | Included in data model       |
| Gross Margin | Net Sales – COGS                                       | Main profitability metric    |
| Net Profit   | Gross Margin – operating/other expenses                | Bottom line metric           |
| GM%          | (Gross Margin ÷ Net Sales) × 100                       | Trend tracked yearly         |

_All calculations aligned with AtliQ’s business flow and data structure, as reflected in the Power BI model._

---

## 5. Profit & Loss Statement (P&L) Structure

- **Flow:** Net Sales → COGS → Gross Margin → Expenses → Net Profit
- **Discounts:** Both pre-invoice and post-invoice deductions (e.g., rebates, promotions) are included in Net Price and Net Sales.
- **Fiscal Metrics:** Year-to-Date (YTD) and Year-to-Go (YTG) implemented for progress and forecasting.

**![Insert P&L Visual or KPI Matrix Screenshot Here](../images/pnl_matrix.png)**

---

## 6. Power BI Implementation

- **Dynamic KPIs:** Net Sales, Gross Margin %, Net Profit %.
- **Matrix & Trend Visuals:** Detailed P&L by period, region, product.
- **Slicers/Filters:** Fiscal year, market, product segment, customer.
- **Navigation:** Bookmark buttons for page/section switching (Finance, Sales, etc.).
- **YTD/YTG Logic:** Fiscal year-driven, based on AtliQ’s September–August cycle.

**![Insert Dashboard Screenshot Here](../images/dashboard_overview.png)**

---

## 7. Business Insights & Value Delivered

- **Explosive Sales Growth:** Net Sales nearly tripled from 2020 to 2021.
- **Margin Trend:** Gross Margin % declined, highlighting cost/price pressures.
- **Target Gap:** Dashboard flagged ~9% shortfall vs. sales targets, regionally highlighted.
- **Performance Drivers:** Top contributors (e.g., Amazon, AtliQ online) and underperforming segments identified.
- **Actionability:** Enabled earlier management interventions—resource reallocation, cost control, and sales strategy adjustment.

**![Insert Insights or Top Performer Chart Screenshot Here](../images/insights_chart.png)**

---

## 8. Technical Approach & Skills Demonstrated

- Power Query for ETL and fiscal logic.
- Star schema modelling.
- Advanced DAX for P&L, YTD, YOY, and KPIs.
- Dashboard UX: dynamic filters, conditional formatting, custom navigation.
- Data reconciliation and accuracy validation.

---

## 9. Relevance to Finance Job Roles

- Real-world financial analysis (P&L, gross/net calculations, margin analysis).
- Automation of reporting and accuracy—critical for accountant, bookkeeper, or analyst roles.
- Transferable business skills: communication, attention to detail, and data-driven insight generation.

---

## 10. Conclusion & Next Steps

This project demonstrates my ability to modernize and automate financial reporting, deliver real insights from raw business data, and apply financial logic that meets industry needs.  
**See the rest of this repository for code samples, screenshots, and additional documentation.**

---

