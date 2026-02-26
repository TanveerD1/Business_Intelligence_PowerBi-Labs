# Business Intelligence & Power BI Labs

A comprehensive collection of Power BI projects and labs demonstrating data visualization, dashboard design, business intelligence best practices, and advanced data preparation techniques.

## Overview

This repository contains laboratory assignments and projects completed during the Business Intelligence course. Each project showcases practical applications of Power BI Desktop for creating interactive dashboards, analyzing sales data, deriving business insights, and implementing professional data governance practices.

**Student:** Tanveer (Student ID: 752)  
**Course:** DSA3050A – Business Intelligence & Data Visualization

---

## 📑 Quick Navigation

### 📌 Assignment Summaries & Links
| Assignment | Documentation | PDF | Status |
|------------|---------------|-----|--------|
| **Assignment 1** | [Sales Dashboard README](Assignment_1/README.md) | [assignment_1.pdf](Assignment_1/assignment_1.pdf) | ✅ Complete |
| **Assignment 2** | [Power Query Lab README](Assignment_2/README.md) | [View Submission Folder](Assignment_2/PowerBI_FIles/Submission) | ✅ Complete |
| **Mid-Semester** | [UK Accidents Analysis README](Mid-Semester/README.md) | [Tanveer_PowerBI-MIDSEM.pdf](Mid-Semester/Tanveer_PowerBI-MIDSEM.pdf) | ✅ Complete |
| **Quiz 1** | — | [Tanveer_DSA3050A Quiz 1 Submission.pdf](Quiz_1/Tanveer_DSA3050A%20Quiz%201%20Submission.pdf) | ✅ Complete |

---

## 📊 Project Details

### Assignment 1: Sales Performance Dashboard

**Overview:** A comprehensive Power BI dashboard analyzing sales metrics across regions, products, and time periods with real-time interactivity.

**Key Features:**
- 10 professional interactive visualizations including KPIs, charts, and data tables
- 3 dynamic slicers enabling multi-dimensional filtering (Region, Product Category, Date)
- Cross-filtered analysis with automatic visual updates across all charts
- Professional styling using Power BI's Simple Gray theme
- Live interactive dashboard published to Power BI Service for real-time access

**Technologies Used:**
- Power BI Desktop
- Excel data source (Sales_Data.xlsx)
- DAX formulas for KPI calculations

**Deliverables:**
- 📋 [Full Documentation](Assignment_1/README.md)
- 📊 Sales_Dashboard.pbix (Power BI Desktop file)
- 📁 Sales_Data.xlsx (Source dataset)
- 📄 [assignment_1.pdf](Assignment_1/assignment_1.pdf) (Assignment specification)
- 🖼️ Dashboard screenshot (image.png)

**Live Dashboard:** 🔗 [View Interactive Dashboard in Power BI Service](https://app.powerbi.com/groups/me/reports/28562300-039e-4b12-af23-b08273465ea9/964cc932e6a00dd50d4c?experience=power-bi)

---

### Assignment 2: Power Query Data Preparation Lab

**Overview:** An advanced data transformation project demonstrating professional ETL workflows, data quality management, and dimensional modeling using Power Query.

**Key Features:**
- **Data Ingestion & Staging** - Multi-file import and query organization
- **Data Profiling & Quality Assessment** - Comprehensive quality checks and issue identification (26% missing value resolution)
- **Data Cleaning & Standardization** - Text normalization, type enforcement, and missing value handling using advanced formulas
- **Data Integration** - Strategic merge operations and lookup table relationships
- **Business Transformations** - Calculated metrics (Total Sales, Profit Margins, Performance Bands)
- **Star Schema Design** - Fact table (stagedSales) and dimension tables (stagedProducts, stagedRegions)
- **Data Governance & Audit** - Quality flags, audit queries, and data load control mechanisms

**Datasets Processed:**
- AfriRetail_Sales_Dirty → stagedSales (Fact Table)
- AfriRetail_Products_Dirty → stagedProducts (Dimension Table)
- AfriRetail_Regions_Dirty → stagedRegions (Dimension Table)

**Key Transformations:**
- Fixed invalid data types (Date, Numeric columns)
- Resolved 26% missing values in Sales Amount through calculated replacement
- Flagged invalid quantities (negative values)
- Imputed missing Unit Prices using strategic averages
- Standardized text fields (trim, clean, case normalization)
- Implemented 14+ Power Query steps with full documentation
- Created complete audit trail for data quality

**Deliverables:**
- 📋 [Full Documentation with Screenshots](Assignment_2/README.md)
- 📦 [Complete Submission Files](Assignment_2/PowerBI_FIles/Submission) (includes .pbix and supplementary files)
- 🖼️ 16 step-by-step transformation screenshots
- 📊 Overview and data quality assessment visuals

---

### Mid-Semester Project: UK Road Accident Analysis

**Overview:** A comprehensive end-to-end Business Intelligence project analyzing UK road accident data (2005–2015) using Power BI, demonstrating the complete BI lifecycle from data preparation through dashboard development.

**Dataset Information:**
- **Source:** Kaggle - [UK Car Accidents 2005-2015](https://www.kaggle.com/datasets/silicon99/uk-car-accidents-2005-2015)
- **Provider:** UK Department for Transport
- **Records:** 1.7+ million accident records
- **Time Period:** 2005–2015

**Project Workflow:**
1. Dataset Selection & Analysis
2. Data Cleaning & Transformation
3. Star Schema Modeling
4. DAX Metrics & Calculations
5. Interactive Dashboard Design
6. Publication to Power BI Service

**Key Components:**
- Data quality assessment and remediation
- Dimensional model design
- Executive dashboard with actionable insights
- Professional publishing and sharing

**Deliverables:**
- 📋 [Project Summary & Overview](Mid-Semester/README.md)
- 📄 [**Full Submission PDF**](Mid-Semester/Tanveer_PowerBI-MIDSEM.pdf) ⭐ (Complete project documentation)
- 🔗 [Live Dashboard](https://app.powerbi.com/links/VygqYQWzGS?ctid=16d83ee6-254a-469d-a6cc-54e2ca2313e7&pbi_source=linkShare) (Interactive analysis)
- 🖼️ Dataset preview and analysis screenshots

---

### Quiz 1: Power BI Fundamentals Assessment

**Overview:** A quick assessment covering core Power BI concepts and practical lab exercises.

**Content:**
- Conceptual questions on Power BI fundamentals
- Practical lab exercise demonstrating BI skills

**Deliverable:**
- 📄 [**Complete Quiz Submission PDF**](Quiz_1/Tanveer_DSA3050A%20Quiz%201%20Submission.pdf)

---

## 📁 Repository Structure

```
Business_Intelligence_PowerBi-Labs/
│
├── Assignment_1/
│   ├── README.md                    # Detailed documentation
│   ├── assignment_1.pdf             # Assignment specification
│   ├── Sales_Dashboard.pbix         # Power BI Desktop file
│   ├── Sales_Data.xlsx              # Source dataset
│   └── image.png                    # Dashboard screenshot
│
├── Assignment_2/
│   ├── README.md                    # Detailed documentation with 16 screenshots
│   ├── PowerBI_FIles/
│   │   ├── Submission/              # Complete submission files
│   │   │   ├── ASSIGNMENT_2(ZIP).zip
│   │   │   └── (non-zipped backup files)
│   │   └── [supplementary .pbix files]
│   ├── image.png through image-16.png  # Transformation step screenshots
│   ├── screenshot1.png              # Overview screenshot
│   └── [additional documentation]
│
├── Mid-Semester/
│   ├── README.md                    # Project summary
│   ├── Tanveer_PowerBI-MIDSEM.pdf  # **Full submission (primary deliverable)**
│   ├── image.png through image-28.png  # Analysis and dashboard screenshots
│   └── [supporting visuals]
│
├── Quiz_1/
│   └── Tanveer_DSA3050A Quiz 1 Submission.pdf  # Quiz submission
│
├── LICENSE                          # Repository license
├── README.md                        # This file (main overview)
└── .git/                            # Version control
```

---

## 🛠️ Technology Stack

| Technology | Purpose |
|-----------|---------|
| **Power BI Desktop** | Dashboard design, data modeling, and visualization (June 2024+) |
| **Power Query** | ETL, data transformation, and data cleaning |
| **DAX (Data Analysis Expressions)** | Calculated measures, KPIs, and advanced metrics |
| **Excel** | Source data and supplementary analysis |
| **Power BI Service** | Publishing, sharing, and interactive reporting |

---

## 📚 Key Concepts & Learnings

- ✅ **Dashboard Design:** Professional visualization design with intuitive user experience
- ✅ **Interactive Filtering:** Dynamic slicers and cross-filtering for multi-dimensional analysis
- ✅ **Data Quality Management:** Profiling, assessment, and systematic issue resolution
- ✅ **ETL Best Practices:** Power Query transformations with proper data governance
- ✅ **Star Schema Design:** Dimensional modeling for enterprise analytics
- ✅ **Data Cleaning:** Handling missing values, standardization, and type validation
- ✅ **DAX Calculations:** Creating business metrics and KPIs
- ✅ **Data Documentation:** Comprehensive step-by-step documentation for reproducibility
- ✅ **Publishing & Sharing:** Deploying dashboards to Power BI Service for organizational access

---

## 🚀 How to Use This Repository

1. **Browse Documentation:** Start with this README for an overview, then visit individual assignment folders for detailed explanations
2. **Open Power BI Files:** Download `.pbix` files from Assignment 1 or Assignment 2 and open them in Power BI Desktop (June 2024 or later)
3. **Review Screenshots:** Each assignment includes step-by-step screenshots showing the complete workflow
4. **View Live Dashboards:** Click the Power BI Service links for interactive exploration of published dashboards
5. **Access PDFs:** Use the quick links above to review assignment specifications and submission documents
6. **Study Datasets:** Review source Excel files (Assignment 1) to understand data structure and quality

---

## 📖 How to Access Each Project

| Project | Access Method | Files |
|---------|--------------|-------|
| **Assignment 1** | Open `.pbix` in Power BI Desktop OR view live dashboard link | [Folder](Assignment_1/) |
| **Assignment 2** | Review README with screenshots, extract submission files from zip | [Folder](Assignment_2/) |
| **Mid-Semester** | Read PDF submission for complete documentation, view live dashboard | [Folder](Mid-Semester/) |
| **Quiz 1** | Review PDF submission document | [Folder](Quiz_1/) |

---

## ℹ️ Additional Resources

- **Power BI Official Documentation:** Learn more about Power BI Desktop, Power Query, and DAX
- **Microsoft Learn:** Free training courses on Power BI and data analysis
- **Kaggle:** Explore additional datasets for practice projects

---

## 📜 License

This repository is licensed under the terms specified in the [LICENSE](LICENSE) file.

---

## 👤 Contact & Questions

For questions about repository contents, project implementations, or reproducibility issues, please contact the repository owner.

**Course:** DSA3050A – Business Intelligence & Data Visualization  
**Student:** Tanveer (752)  
**Last Updated:** February 2026
