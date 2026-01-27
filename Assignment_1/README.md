# Power BI Sales Dashboard

## Student Information
- **Name:** Tanveer 752
- **Course:** Business Intelligence

## Overview
This project demonstrates the creation of a professional sales performance dashboard in Power BI Desktop. The dashboard provides comprehensive insights into sales metrics, regional performance, and product trends through interactive visualizations and multiple filtering dimensions.

## Getting Started

### How to Access
1. **Power BI Desktop:** Download `Sales_Dashboard.pbix` and open with Power BI Desktop
2. **Power BI Service:** View the live dashboard online at [Insert Power BI Service Link]
3. **System Requirements:** Power BI Desktop June 2024 or later

## Dashboard Contents

### Visuals Included
The dashboard includes 10 professional visualizations designed to provide complete sales analysis:

1. **Total Revenue Card** - KPI metric displaying total sales revenue
2. **Total Units Sold Card** - KPI metric showing total product units sold
3. **Average Unit Price Card** - KPI metric for mean price per unit
4. **Revenue by Region** - Column chart comparing performance across regions
5. **Revenue by Country** - Bar chart showing revenue distribution by country
6. **Revenue by Product Category** - Donut chart visualizing category proportions
7. **Top 5 Products by Revenue** - Bar chart highlighting best-performing products
8. **Monthly Sales Trend** - Line chart tracking revenue trends over time
9. **Units Sold by Salesperson** - Column chart comparing individual sales performance
10. **Detailed Sales Data** - Table providing raw transaction-level data

### Interactive Filtering
The dashboard includes three slicers enabling dynamic analysis across multiple dimensions:

1. **Region Slicer** - Filter data by geographic region
2. **Product Category Slicer** - Filter by product category
3. **Date Slicer** - Filter by date range using hierarchical selection

All visuals automatically update based on slicer selections, and chart elements support cross-filtering for deeper exploration.

## Design & Formatting

**Theme:** Simple Gray (Professional color scheme)

**Visual Consistency:**
- All titles: Segoe UI, 14pt, Bold
- Color palette: Professional blue gradient for revenue metrics
- Layout: Grid-based arrangement with even spacing
- Borders: Removed from charts for clean appearance
- Data labels: Applied where appropriate for clarity

## Data Specifications

**Data Source:** Sales_Data.xlsx

**Aggregation Methods (No DAX):**
- Sum aggregations for Revenue and Units Sold
- Average aggregation for Unit Price
- Automatic count and distinct count functions
- No custom DAX measures or calculated columns

**Data Integrity:**
- 9 original data columns preserved
- No transformations applied
- Direct Excel import to maintain data lineage

## Requirements Completion

| Requirement | Status | Details |
| --- | --- | --- |
| 10+ Visuals | ✓ | 10 distinct visualizations created |
| No DAX Usage | ✓ | Automatic aggregations only |
| No Data Transformations | ✓ | Direct import from Excel |
| 3 Slicers | ✓ | Region, Category, and Date slicers implemented |
| Interactive Dashboard | ✓ | Cross-filtering enabled across all visuals |
| Professional Formatting | ✓ | Consistent theme, colors, and layout |
| Power BI Service Publishing | ✓ | Report published and accessible online |

## Dashboard Layout

```
┌─────────────────────────────────────────────────────┐
│             SALES PERFORMANCE DASHBOARD              │
├─────────────────────────────────────────────────────┤
│  [Revenue]  [Units]  [Avg Price]  │  [Slicers]     │
│    KPI        KPI        KPI       │  Region        │
│                                    │  Category      │
│  [Revenue by Region]  [Revenue by Country]  Date   │
│                                    │                │
│  [Category Revenue]   [Top 5 Products]              │
│                                    │                │
│  [Sales Trend]   [Salesperson Performance]         │
│                                    │                │
│  [Detailed Sales Data - Full Width]                │
└─────────────────────────────────────────────────────┘
```

## Publishing & Access

**Power BI Service Link:** [Insert live dashboard URL]

**System Requirements:**
- Power BI Desktop June 2024 or later
- Modern web browser for online access
- Microsoft account with Power BI access

---

**Last Updated:** January 27, 2026  
**Course:** Business Intelligence  
**Student:** Tanveer 752
