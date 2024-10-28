# Car Repair Service Company Data Analysis

This repository contains an in-depth analysis of a car repair service company, with a special focus on supplier performance, customer satisfaction, and overall sales growth. The analysis is driven by data visualizations and insights generated through **Power BI** dashboards.

---

## 1. Background and Overview

The dataset belongs to a company in the vehicle maintenance industry. The business model involves collecting vehicles from customers, outsourcing the repairs to third-party suppliers, and delivering the repaired vehicles back. The company operates in multiple regions and has been active for over six years. This analysis aims to uncover insights to optimize business performance, focusing on the following areas:

- **Sales Growth**: Analyze yearly and monthly sales patterns to identify trends.
- **Supplier Comparison**: Compare the performance of suppliers based on revenue, customer satisfaction, and job delivery times.
- **Product and Service Analysis**: Analyze which car models and job types drive the most revenue and customer satisfaction.

---

## 2. Executive Summary

This data analysis provides insights into the car repair company’s performance across multiple metrics such as sales growth, supplier efficiency, and customer satisfaction. 

### Key Findings:

1. **Supplier Performance**: Supplier SP003 generates the highest revenue, maintains the fastest job completion time, and has the highest customer satisfaction.
2. **Sales Trends**: Significant increases in sales were observed in August and September, coinciding with seasonal factors such as the rainy season.
3. **Product and Service Trends**: The **Toyota Camry** was the most serviced car model, and specific job types were linked to higher customer satisfaction.

### Recommendations:

1. **Optimize Supplier Performance**: Prioritize assigning jobs to **Supplier SP003**, who performs the best in terms of job completion time and customer satisfaction.
2. **Targeted Marketing**: Capitalize on the increased demand during the rainy season (August and September) with targeted campaigns.
3. **Improve Service for Lower-Rated Suppliers**: Address areas of improvement for suppliers with lower performance, such as **Supplier SP002**.

---

## 3. Data Structure and Initial Checks

### Entity-Relationship Diagram (ERD)

![ERD](https://github.com/user-attachments/assets/8e0bcb81-2827-450a-8474-2dbf71e4f7db)

The data structure consists of the following tables:

- **Customers**: Contains customer demographics and details.
- **Cars**: Includes car model information.
- **Jobs**: Lists job types and repair details.
- **Suppliers**: Supplier details such as job completion time, revenue per job, and ratings.
- **Sales**: Revenue, job completion times, and other sales metrics.

---

## 4. Analysis Insights

### 4.1 Yearly Growth and Sales Analysis

**Objective**: Analyze overall sales growth over the years and identify key months of high sales activity.

**Key Insight**:
- Sales tend to increase in August and September, coinciding with the rainy season, which typically leads to more vehicle repairs.

#### Visualization:
![Month Revenue](https://github.com/user-attachments/assets/8fb433dd-0942-457c-86e5-67a968881f20)

---

### 4.2 Regional Analysis

**Objective**: Analyze sales and job distribution across different regions.

**Key Insight**:
- The **Omdurman** region has the highest demand for car repair services, followed by **Khartoum**.

#### Visualization:
![Location](https://github.com/user-attachments/assets/af3288e6-9b58-42c6-8ac2-1f567a3e2c60)

---

### 4.3 Product and Service Analysis

**Objective**: Analyze the car models and types of repairs that contribute the most to revenue.

**Key Insight**:
- The **Toyota Camry** is the most serviced car model, contributing significantly to total revenue.
- **Engine repairs** and **bodywork** jobs are associated with higher customer satisfaction compared to other job types.

#### Visualization:
![Revenue Car](https://github.com/user-attachments/assets/27b07068-65ba-4522-8f12-69add901f6cd)

---

### 4.4 Supplier Analysis

**Objective**: Compare the performance of suppliers based on total revenue generated, average job completion time, and customer satisfaction ratings.

#### Supplier Performance Overview

- **Supplier SP003**: 
  - **Total Revenue**: Highest among all suppliers.
  - **Customer Rating**: 4.5/5 (best rating).
  - **Average Job Time**: 2 days (fastest completion time).
  
- **Supplier SP001**:
  - **Total Revenue**: Moderate revenue generation.
  - **Customer Rating**: 4.0/5.
  - **Average Job Time**: 3 days.
  
- **Supplier SP002**:
  - **Total Revenue**: Below average.
  - **Customer Rating**: 3.2/5 (lowest rating).
  - **Average Job Time**: 5 days (longest completion time).

#### Visualization:
![Supplier revenue](https://github.com/user-attachments/assets/6e08ac26-8807-4dba-b5ba-736a1f75c2d4)
![Supplier vs amount per job vs customer rating](https://github.com/user-attachments/assets/653e5484-b319-4c8a-9efb-c04f52825234)

---

### 4.5 Customer Satisfaction by Car Model and Supplier

**Objective**: Analyze customer satisfaction ratings based on the car models serviced and the suppliers used.

**Key Insight**:
- Customers tend to give higher satisfaction ratings for repairs on **Toyota Camry** and **Honda Civic** models.
- There is a clear trend showing that as the average job time increases, customer satisfaction ratings decrease.

#### Visualization:
![Job duration vs Cus rating](https://github.com/user-attachments/assets/959e3547-b98b-4b99-9428-164c446cf4a0)
![Revenue car model vs vs](https://github.com/user-attachments/assets/6aaf2166-f59a-41f5-baa1-d4221b399ac3)

---

## 5. Recommendations

1. **Optimize Supplier Performance**:
   - Focus more jobs towards **Supplier SP003**, as they have the best performance in terms of revenue, job time, and customer ratings.
   - Consider improving **Supplier SP002** through additional training to reduce job time and enhance customer service.

2. **Target Marketing During Rainy Season**:
   - Invest in targeted marketing campaigns in August and September to take advantage of increased demand during the rainy season.

3. **Improve Service for Low-Rating Suppliers**:
   - Address the issues with suppliers who are receiving lower customer satisfaction ratings, particularly **SP002**.

---

## 6. Assumptions and Caveats

1. **Assumption 1**: All missing months or outliers in the data were treated by extrapolating trends from available data.
2. **Assumption 2**: Outlier data points were excluded unless patterns were consistently observed.

---

## Power BI Dashboards

- Download or explore the [Power BI dashboard]() containing:
    1. Main Dashboard - Sales Overview.
    2. Supplier Analysis Dashboard.
    3. Car Model Analysis Dashboard.

---

## Repository Contents

- **/data**: Contains sample datasets used for the analysis.
- **/dashboards**: Power BI dashboard files.

## Getting Started

- Download the dataset from the repository.
- Open the **.pbix** files in **Power BI Desktop** to explore the interactive dashboards.

---

