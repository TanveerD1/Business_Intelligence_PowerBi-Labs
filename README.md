# Business Intelligence & Power BI Labs

A comprehensive collection of Power BI projects and labs demonstrating data visualization, dashboard design, business intelligence best practices, and advanced data preparation techniques.

## Overview

This repository contains laboratory assignments and projects completed during the Business Intelligence course. Each project showcases practical applications of Power BI Desktop for creating interactive dashboards, analyzing sales data, deriving business insights, and implementing professional data governance practices.

**Student:** Tanveer 752  
**Course:** Business Intelligence

---

## Projects

### Assignment 1: Sales Performance Dashboard

A comprehensive Power BI dashboard analyzing sales metrics across regions, products, and time periods.

**Key Features:**
- 10 interactive visualizations including KPIs, charts, and data tables
- 3 dynamic slicers for filtering (Region, Product Category, Date)
- Cross-filtered analysis with automatic visual updates
- Professional styling and formatting using Simple Gray theme
- Live interactive dashboard published to Power BI Service

**Deliverables:**
- Sales_Dashboard.pbix - Power BI Desktop file
- Sales_Data.xlsx - Source dataset
- ssignment_1.pdf - Assignment specification

**Live Dashboard:** [View in Power BI Service](https://app.powerbi.com/groups/me/reports/28562300-039e-4b12-af23-b08273465ea9/964cc932e6a00dd50d4c?experience=power-bi)

[View Full Assignment 1 Details](Assignment_1/README.md)

---

### Assignment 2: Power Query Data Preparation Lab

An advanced Power Query transformation project demonstrating professional data governance, quality assessment, and star schema design for business intelligence.

**Key Features:**
- **Data Ingestion & Staging** - Multi-file import and query organization
- **Data Profiling & Quality Assessment** - Comprehensive quality checks and issue identification
- **Data Cleaning & Standardization** - Text normalization, type enforcement, and missing value handling
- **Data Integration** - Strategic merge operations with lookup tables
- **Business Transformations** - Calculated metrics (Total Sales, Profit, Performance Bands)
- **Star Schema Design** - Dimension tables (dimProducts, dimRegions) and aggregated summary tables
- **Data Governance & Audit** - Quality flags, audit queries, and load control

**Datasets Processed:**
- AfriRetail_Sales_Dirty  stagedSales (Fact Table)
- AfriRetail_Products_Dirty  stagedProducts (Dimension Table)
- AfriRetail_Regions_Dirty  stagedRegions (Dimension Table)

**Key Transformations:**
- Fixed invalid data types (Date, Numeric columns)
- Resolved 26% missing values in Sales Amount through calculated replacement
- Flagged invalid quantities (negative values)
- Imputed missing Unit Prices using averages
- Standardized text fields (trim, clean, case normalization)
- Created profit and performance metrics
- Implemented 14 Power Query steps with full documentation

**Deliverables:**
- Comprehensive README with step-by-step documentation
- 14 screenshots showing each transformation stage
- Audit query isolating problem records
- Analysis-ready star schema model

[View Full Assignment 2 Details](Assignment_2/README.md)

---

### Quiz 1: Quick Assessment

A short Power BI quiz covering core concepts and a small lab exercise.

**Deliverables:**
- a single pdf with all Quiz one requirements

[View Quiz 1 Details](Quiz_1/Tanveer_DSA3050A%20Quiz%201%20Submission.pdf)

---

### Assignment 2: Power Query Data Preparation Lab

---


## Repository Structure

\\\
Business_Intelligence_PowerBi-Labs/
 Assignment_1/
    README.md                 # Assignment 1 documentation
    Sales_Dashboard.pbix      # Power BI desktop file
    Sales_Data.xlsx           # Source data
    assignment_1.pdf          # Assignment specification
    image.png                 # Dashboard screenshot
 Assignment_2/
    README.md                 # Assignment 2 documentation
    image-1.png to image-14.png # Step-by-step transformation screenshots
    screenshot1.png           # Overview screenshot
 Quiz_1/
     [text](<Quiz_1/Tanveer_DSA3050A Quiz 1 Submission.pdf>)
 LICENSE                       # Repository license
 README.md                     # This file
\\\

---

## Technology Stack

- **Power BI Desktop** (June 2024 or later)
- **Power Query** for data transformation and ETL
- **Excel** for source data and data export
- **DAX** (used where applicable for calculated measures)

---

## How to Use This Repository

1. **Navigate to the assignment folder** of interest and open its \README.md\ for specific instructions and context.
2. **Use Power BI Desktop** to open \.pbix\ files where provided; review accompanying data files to validate results.
3. **Review screenshots and documentation** to understand the complete workflow for each assignment.
4. **Consult the LICENSE file** for permitted use and distribution.

---

## Key Learnings

- **Dashboard Design:** Professional visualization design with interactive filtering
- **Data Quality Management:** Profiling, assessment, and systematic issue resolution
- **ETL Best Practices:** Power Query transformations with proper data governance
- **Star Schema Design:** Dimensional modeling for analytics
- **Data Documentation:** Comprehensive step-by-step documentation for reproducibility

---

## Contact

For questions about contents or reproducibility, contact the repository owner.

**License:** See the \LICENSE\ file in the repository root.
