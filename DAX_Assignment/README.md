# 🚗 Adult Income Dataset (1994)

### DAX Assignment

**Course:** DSA3050A – Business Intelligence & Data Visualization
**Student:** Tanveer
**Student ID:** 752

**Link to DASHBOARD:** 

- https://app.powerbi.com/view?r=eyJrIjoiMTg3YmRhMGItNDdlMS00NjUxLTk3MDctMWRmZmMxYWVhM2E5IiwidCI6IjE2ZDgzZWU2LTI1NGEtNDY5ZC1hNmNjLTU0ZTJjYTIzMTNlNyIsImMiOjh9

---
# 📊 Dataset Information

**Source:** UC Irvine Machine Learning repository
**Dataset:** Adult
**Provider:** 1994 census dataset
**Rows:** 48842

Dataset link:
[https://archive.ics.uci.edu/dataset/2/adult](https://archive.ics.uci.edu/dataset/2/adult)


### Proof of Website

![proof of Data/website](image.png)

### Dataset

![dataset_example](image-1.png)

# SECTION A: DATA MODEL VALIDATION 

### Creating Date Table

![created date table dax](image-4.png)

![monthdax](image-5.png)

![quarterdax](image-6.png)

### Creating relationship

![creating relationship between date table and main fact table](image-2.png)

![star schema](image-3.png)

# SECTION B: CORE DAX MEASURES

![where the new measures is](image-7.png)

### Measure 1: Total individuals

![total individuals dax](image-8.png)

### Measere 2: Average worked hours

![average worked hoursdax](image-9.png)

### Measure 3: High Income count

![high income count dax](image-10.png)

### Measere 4: High income percentage

![high income % dax](image-11.png)

### Measure 5: Low income Count

![low income count dax](image-12.png)

# SECTION C: CALCULATED COLUMNS

### Column 1:  Age Group Classification

![age group dax](image-13.png)

### Column 2: Work Hours Category

![work hours category](image-14.png)

### Column 3:  Education Level Group

![edu levl dax](image-15.png)

# SECTION D: FILTER CONTEXT & CALCULATE

### Measure 1: Female High Income percentage

![female high income percentage](image-16.png)

### Measure 2: Percentage of National Average 

![% of national income](image-17.png)

### Measure 3: Professional Contribution

![professional contribution](image-18.png)

### Measure 4: Gender Gap Analysis

![gender income gap dax](image-19.png)

#  SECTION E: ITERATOR FUNCTION

### Total Estimated Income (SUMX)

![SUMX dax](image-20.png)

### Average Education Level by Occupation (AVERAGEX)

![averagexdax](image-21.png)

### Total Capital Activity (SUMX with multiple columns)

![sumxMultiDAX](image-22.png)

# SECTION F: TIME INTELLIGENCE

### Measure 1: Year-to-Date Individuals

![time intel dax 1](image-23.png)

### Measure 2: Previous Quarter (comparing to last period)

![time intel dax 2](image-24.png)

### Measure 3: Quarter-over-Quarter Growth percentage

![time intel dax 3](image-25.png)

### Measure 4: Same Period Last Year

![time intel dax 4](image-26.png)

# SECTION G: VISUAL VALIDATION

![visual](image-27.png)

![alt text](image-28.png)


