# **Medical Inventory Optimization**

## **Introduction**

_Analyzing bounce rate and inventory management to support strategic purchasing and inventory decisions using SQL, Python, and Power BI._

---

## **Overview**

This project aims to tackle the rising bounce rate within a healthcare organisation, which has been causing patient dissatisfaction. The primary aim is to decrease the bounce rate by a minimum of 30%, while also cutting down on inventory expenses and expecting a revenue boost of at least 20 lacs INR. It focuses on the critical business challenge of excessive medical inventory costs by developing a data-driven optimization model. The goal was to identify inefficiencies, minimize waste from expired items, reduce bounce rate, and recommend a cost-effective inventory strategy. Employing a Data Analytics Project Management Methodology, this project will work with a dataset comprising 14,218 rows and 14 columns, specifically targeting the Supply Chain Management sector.

---

## **Project Scope**

### **Background Information**

Efficient management of medical inventory through development of forecasting model holds immense importance for healthcare facilities worldwide. Inaccurate forecasting of drug demand can lead to issues like stockouts, overstocking, and increased expenses, all of which directly impact patient care. By harnessing advanced machine learning models, the proposed system seeks to refine medical inventory management practices, aiming to enhance stock availability, reduce bounce rates, elevate customer satisfaction, and minimize wastage in inventory costs.

**Business Problem:** 
- Drug shortages in stocks
- Increase of bounce rate
  
**Business Objective:** 
- Minimize bounce rate.
- Maximize availability of drug, customer satisfaction, and profits.

---

## **Dataset**

The medical dataset comprises 14,218 records and includes essential columns that capture various aspects of pharmaceutical transactions, patient behavior, and inventory management. Here is an overview of the dataset:

- **Typeofsales**: Indicates the type of drug sale (sold or returned).
- **Patient_ID**: Unique identifier for patients.
- **Specialisation**: Name of the specialization (e.g., Cardiology).
- **Dept**: Pharmacy department related to the formulation.
- **Dateofbill**: Date of purchase of medicine.
- **Quantity**: Quantity of the drug purchased.
- **ReturnQuantity**: Quantity of drug returned by patients.
- **Final_Cost**: Final cost of the drug (including quantity).
- **Final_Sales**: Final sales amount of the drug.
- **RtnMRP**: Maximum Retail Price (MRP) of returned drugs.
- **Formulation**: Type of formulation.
- **DrugName**: Generic name of the drug.
- **SubCat**: Subcategory (Type) of the category of drugs.
- **SubCat1**: Subcategory (condition) of the category of drugs.

### Missing Values
The dataset contains missing values in several columns:
- **Formulation**: 4.59% missing values.
- **DrugName**: 11.73% missing values.
- **SubCat**: 11.73% missing values.
- **SubCat1**: 11.9% missing values.

Addressing these missing values through imputation or removal is crucial to ensure data integrity and reliability for subsequent data analysis processes.

---

## **Tools & Technologies**

- SQL (Common Table Expressions, Joins, Filtering)
- Python (Pandas, Matplotlib, Seaborn, SciPy)
- Power BI (Interactive Visualizations)
- GitHub

---

## **Data Preprocessing**

### **Objectives**
- Data Cleaning: Identify errors, inconsistencies, null values and missing values in the dataset.
- Data Transformation: Convert data into an appropriate format or scale for analysis or modeling.
- Feature Engineering: Create new relevant features or variables from the existing data to improve the performance of machine learning models.<br>

### **Methods Implemented**
1. Type Casting
2. Duplication Handling
3. Handling Missing Values
4. Handling Null Values
5. Data manipulation

---

## **Descriptive Statistics**
1. First Moment Business Decision: Measure of Central Tendency
2. Second Moment Business Decision: Measure of Dispersion
3. Third Moment Business Decision: Skewness
4. Forth Moment Business Decision: Kurtosis

- **[Click here to view full documentation of data preprocessing (Python)](https://github.com/maverickcodes1/medical-inventory-optimization-sql-python-powerbi/blob/main/Data_Preprocessing%20(MIO%20-%20Python).py)**
- **[Click here to view full documentation of data preprocessing (SQL)](https://github.com/maverickcodes1/medical-inventory-optimization-sql-python-powerbi/blob/main/Data_Preprocessing%20(MIO%20-%20SQL).sql)**

---

## **Exploratory Data Analysis (EDA)**

### **1. Univariate Analysis**

<p align="center">
  <kbd><img width="500" src="https://github.com/maverickcodes1/medical-inventory-optimization-sql-python-powerbi/blob/main/Images/Screenshot%202025-10-23%20221728-1.png"></kbd> <br>
  Figure 1 — Box Plot
</p>
<br>

- Each boxplot shows a dense cluster of values near the lower end with long whiskers and multiple outliers stretching upward. This indicates right-skewed distributions, meaning most transactions are low in value, but a few are exceptionally high.

- All five variables exhibit numerous outliers, especially Final_Cost and Final_Sales, which have visibly extended tails. These outliers could represent bulk purchases, high-value prescriptions, or rare return events.

- While the central boxes for ReturnQuantity and RtnMRP are tightly packed, the outliers are far removed, suggesting rare but significant return events.
- This could point to operational inefficiencies, product defects, or policy-driven returns that warrant further investigation. Segmenting these cases could help uncover patterns in product performance or customer behavior.

<p align="center">
  <kbd><img width="600" src="https://github.com/maverickcodes1/medical-inventory-optimization-sql-python-powerbi/blob/main/Images/Screenshot%202025-10-23%20222535-1.png"></kbd> <br>
  Figure 2 — Histogram
</p>
<br>

- The histograms for Formulation and DrugName show a long tail, with a few items appearing very frequently and many others appearing rarely.
- This suggests a dominance of certain formulations and drugs in the dataset — likely common prescriptions or high-demand products. Rare entries may represent niche treatments or specialized formulations worth flagging for deeper analysis.

- The SubCat histograms reveal that certain therapeutic categories — like “Vitamins Used in Substance Dependence” — occur far more often than others.
- This points to a concentration of prescriptions in specific health domains, possibly driven by regional health trends or institutional focus. Understanding this distribution can help optimize inventory, marketing, or research efforts.

### **2. Bivariate Analysis**

<p align="center">
  <kbd><img width="500" src="https://github.com/maverickcodes1/medical-inventory-optimization-sql-python-powerbi/blob/main/Images/Screenshot%202025-10-23%20221452-1.png"></kbd> <br>
  Figure 3 — Scatter Plot
</p>
<br>

- The Quantity vs ReturnQuantity plot shows most data points clustered near the origin, with low return quantities even for high sales volumes.
- This suggests that returns are rare, indicating either strong product reliability or strict return policies. Beneficial to explore whether specific drugs or departments that deviate from this pattern.

- Both Quantity vs Final_Cost and Quantity vs Final_Sales plots show dense clusters near the origin and scattered outliers.
- This implies that cost and sales don’t increase proportionally with quantity — possibly due to discounts, tiered pricing, or bundled offers. Beneficial to consider engineering features like unit cost or sales per item to normalize these effects.

- The Final_Cost vs Final_Sales plot displays a diagonal trend, indicating a direct and consistent relationship, which is an indicator of strong positive correlation between Final_Cost and Final_Sales
- This suggests that sales are tightly linked to cost, which is useful for margin analysis and anomaly detection. Any deviation from this trend could signal pricing errors, promotional impacts, or data quality issues.

---

## **Key Findings**

