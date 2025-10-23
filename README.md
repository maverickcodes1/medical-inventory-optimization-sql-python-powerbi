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

## **Data Preprocessing**

### **Objectives**
- Data Cleaning: Identify errors, inconsistencies, null values and missing values in the dataset.
- Data Transformation: Convert data into an appropriate format or scale for analysis or modeling.
- Feature Engineering: Create new relevant features or variables from the existing data to improve the performance of machine learning models.<br>

8 data preprocessing methods were implemented:
1. Type Casting
2. Duplication Handling
3. Handling Missing Values
4. Handling Null Values
5. Data manipulation

## **Descriptive Statistics**
1. First Moment Business Decision: Measure of Central Tendency
2. Second Moment Business Decision: Measure of Dispersion
3. Third Moment Business Decision: Skewness
4. Forth Moment Business Decision: Kurtosis

**[Click here to view full documentation of data preprocessing (Python)](https://github.com/maverickcodes1/medical-inventory-optimization-sql-python-powerbi/blob/main/Data_Preprocessing%20(MIO%20-%20Python).py)**
**[Click here to view full documentation of data preprocessing (SQL)](Data_Preprocessing (MIO - SQL).sql)**
