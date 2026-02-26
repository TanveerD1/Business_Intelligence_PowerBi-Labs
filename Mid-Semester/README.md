# 🚗 UK Road Accident Analysis (2005–2015)

### Power BI Business Intelligence Project

**Course:** DSA3050A – Business Intelligence & Data Visualization
**Student:** Tanveer
**Student ID:** 752

---

## 📌 Project Overview
## 📊 Dataset Information
This project demonstrates a complete end-to-end Business Intelligence workflow using Power BI.

The objective was to analyze UK road accident data and build an executive dashboard that supports decision-making through:

* Data cleaning & transformation
* Star schema modelling
* DAX metric creation
* Interactive dashboard design
![Dataset preview](image.png)
![Dataset sample](image-1.png)
This project follows a full BI lifecycle:

> Dataset Selection → Data Preparation → Data Modelling → Dashboard Development → Publishing

---

## 📊 Dataset Information

**Source:** Kaggle
**Dataset:** UK Car Accidents (2005–2015)
**Provider:** UK Department for Transport
**Rows:** 1.7+ million accident records

Dataset link:
[https://www.kaggle.com/datasets/silicon99/uk-car-accidents-2005-2015](https://www.kaggle.com/datasets/silicon99/uk-car-accidents-2005-2015)

[![alt text](image.png)]
[![alt text](image-1.png)]
### Dataset Structure
The dataset contains three main tables:

1. **Accidents0515.csv**

   * One row per accident

2. **Vehicles0515.csv**

   * Multiple vehicles per accident
   * Foreign Key: `Accident_Index`

![Before loading preview](image-2.png)
3. **Casualties0515.csv**

   * Multiple casualties per accident
   * Foreign Key: `Accident_Index`

![After loading preview](image-3.png)
This structure naturally supports a **Star Schema**.


# 🔄 PART A — Data Preparation (Power Query)

All datasets were transformed using Power Query.

---

## 1️⃣ Dataset Loading

### Before Loading

```
![Date type correction step 1](image-4.png)
[![alt text](image-2.png)]
```

![Date type correction step 2](image-5.png)
### After Loading into Power BI

[![alt text](image-3.png)]
```

---

## 🟦 DIM_Accidents Transformations

### ✔ Date Type Correction

Problem: Date column stored as text.

Action:

* Converted `Date` column to proper Date type.
![Extract year/month/quarter](image-6.png)

```
```

```
[![alt text](image-5.png)]
```

---

![Duplicate validation](image-7.png)
### ✔ Extract Year, Month, Quarter


* Year
* Month Name
* Month Number
* Quarter

Purpose:
Enables time intelligence analysis.

```
![Missing values handling](image-9.png)
[![alt text](image-6.png)]
```
---

### ✔ Duplicate Validation

Primary Key: `Accident_Index`

Removed duplicates to ensure uniqueness.

```
[![alt text](image-7.png)]

```
![Severity labels standardized](image-10.png)

---
### ✔ Handling Missing Values

Identified null geographic values.

Action:

* Removed rows with null latitude/longitude.

```
[![alt text](image-9.png)]
![Removed unnecessary columns](image-11.png)
```


### ✔ Standardizing Severity Codes

Original Codes:

* 1 = Fatal
![Final applied steps](image-12.png)
* 2 = Serious
* 3 = Slight
Replaced numeric codes with readable labels.

```
[![alt text](image-10.png)]
```

---

### ✔ Removed Unnecessary Columns
![Removed invalid driver ages](image-13.png)

Removed:
* Location_Easting_OSGR
* Location_Northing_OSGR
* Technical fields not required for analysis

```
[![alt text](image-11.png)]
```

---

![Vehicle type standardization](image-14.png)
### ✔ Final Applied Steps


```
[![alt text](image-12.png)]
```

---

## 🟦 FACT_Vehicles Transformations

### ✔ Removed Invalid Driver Ages

* Converted `-1` to null
* Removed null rows
![Driver age group creation](image-15.png)

```
```

---

### ✔ Standardized Vehicle Type Codes

Converted numeric codes to readable categories:

* Pedal Cycle
![Gender codes standardized](image-16.png)
* Motorcycle
* Car
```
[![alt text](image-14.png)]
```

---

### ✔ Created Driver Age Group

Custom Column:

```
![Casualty age groups](image-17.png)
if [Age_of_Driver] < 25 then "Under 25"
else if [Age_of_Driver] < 45 then "25–44"
else "65+"
```

```
[![alt text](image-15.png)]
```
![Query dependency view](image-18.png)

---
## 🟦 FACT_Casualties Transformations

### ✔ Standardized Gender Codes

* 1 → Male
* 2 → Female

```
[![alt text](image-16.png)]
```

---

### ✔ Created Casualty Age Groups

```
else if [Age_of_Casualty] < 30 then "Young Adult"
else if [Age_of_Casualty] < 60 then "Adult"
else "Senior"
```

```
[![alt text](image-17.png)]
```

---

![Model relationships diagram](image-19.png)
### ✔ Query Dependency View


```
[![alt text](image-18.png)]
```

---

# 🏗 PART B — Data Modelling

## ⭐ Star Schema Design

### Fact Tables:
![Date dimension preview](image-20.png)

* `Fact_Vehicles`

### Dimension Tables:

* `Dim_Accidents`
* `Dim_Date`
* `Dim_Location`

---

## 🔗 Relationships
![Location dimension preview](image-21.png)

* Dim_Accidents (1) → Fact_Vehicles (Many)
* Dim_Date → Dim_Accidents
* Dim_Location → Dim_Accidents

No direct relationship between fact tables (avoids ambiguity).

```
[![alt text](image-19.png)]
```

---

## 📅 Date Dimension Creation

Created a proper Date dimension including:
![KPI section screenshot](image-22.png)

* Date
* Month Name
* Month Number
* Quarter

```
[![alt text](image-20.png)]
```

---
![Trend analysis chart](image-23.png)

## 📍 Location Dimension
Created a location table with:

* Latitude
* Longitude
* Location_ID (Index key)

![Comparative analysis chart](image-24.png)
```
[![alt text](image-21.png)]

---

# 📈 PART C — Dashboard Development

## 🎯 KPI Section
![Severity distribution donut](image-25.png)

Measures Created (DAX):
* Total Accidents
* Total Vehicles
* Total Casualties
* Fatal Accidents
* Fatality Rate (%)

![Geographic visualization map](image-26.png)
```
[![alt text](image-22.png)]

---

## 📉 Trend Analysis

Line Chart: Accidents by Year

Insight:
Accident numbers decline over time, indicating improvements in road safety.

```
[![alt text](image-23.png)]
```

---
## 📊 Comparative Analysis

Bar Chart: Accidents by Severity

```
[![alt text](image-24.png)]
```

---
## 🥧 Distribution Visualization

Donut Chart: Severity Distribution

```
[![alt text](image-25.png)]
```
---

## 🗺 Geographic Visualization

Map: Accidents by Latitude/Longitude

```
[![alt text](image-26.png)]
```
---

## 🎛 Interactive Slicers

Slicers Included:

* Year
* Severity
* Month


```
[![alt text](image-27.png)]
```

---

# 🚀 PART D — Publishing


```
[![alt text](image-28.png)]
```

---

## 🔗 Live Dashboard

Power BI Public Link:

👉 [https://app.powerbi.com/links/VygqYQWzGS?ctid=16d83ee6-254a-469d-a6cc-54e2ca2313e7&pbi_source=linkShare]

---

# 🧠 Key Insights

* Slight accidents dominate total incidents.
* Most accidents involve two vehicles.
* Urban areas show higher clustering.
* Fatality rate remains relatively low compared to total volume.
* Accident frequency shows a downward trend from 2005–2015.

---

# 🏆 Skills Demonstrated

* Data Cleaning & Transformation (Power Query)
* Dimensional Modelling (Star Schema)
* DAX Calculations
* Dashboard UX Design
* Business Insight Communication
* Power BI Service Deployment

---

# 📌 Tools Used

* Power BI Desktop
* Power Query
* DAX
* Power BI Service
* VS Code (Data inspection)

---


