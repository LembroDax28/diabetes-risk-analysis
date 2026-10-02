# **Diabetes Risk Analysis**



This project is part of my internship work in data analysis. The project focuses on working with a diabetes risk dataset and preparing it for further analysis by performing data acquisition, exploration, cleaning, and preprocessing.



### **Project Overview**



The dataset contains information about patients, including demographic details, lifestyle factors, and health-related measurements. The main goal of the project is to identify and handle data quality issues before using the dataset for further analysis and visualization.



### Week 1 — Data Cleaning and Preprocessing



The first week of the project focuses on:



* Acquiring a public diabetes risk dataset
* Understanding the structure and contents of the dataset
* Checking data types and categorical values
* Identifying missing values
* Checking for duplicate records
* Verifying patient IDs
* Detecting potential numerical outliers using the IQR method
* Investigating potential outliers using box plots
* Handling missing categorical values
* Validating the cleaned dataset
* Exporting the cleaned dataset for further analysis



#### Missing Value Handling



Missing values were found in the following categorical columns:



* smoking\_status
* alcohol\_consumption
* income\_bracket



These missing values were replaced with 'Unknown' so that the records could be retained without introducing assumptions about the missing information.



#### Outlier Detection



Potential numerical outliers were identified using the **Interquartile Range (IQR)** method.

The following numerical variables were examined:



* Age
* BMI
* Hours of sleep per night
* Stress level
* Fasting blood sugar
* HbA1c level
* Systolic blood pressure
* Diastolic blood pressure
* Waist circumference



Potential outliers were investigated using box plots, particularly for BMI and fasting blood sugar. The detected values were not automatically removed because unusual health measurements may represent valid observations rather than erroneous data.



#### Dataset



The dataset contains **15,000 records and 19 columns**.



Some of the main variables include:



* patient\_id
* age
* gender
* city
* bmi
* family\_history\_diabetes
* physical\_activity\_level
* diet\_type
* smoking\_status
* alcohol\_consumption
* hours\_sleep\_per\_night
* stress\_level
* fasting\_blood\_sugar
* hba1c\_level
* blood\_pressure\_systolic
* blood\_pressure\_diastolic
* waist\_circumference\_cm
* income\_bracket
* diabetes\_risk



**Dataset source**: [Diabetes-Risk-Analysis-Dataset](https://www.kaggle.com/datasets/mansiaggarwal88/diabetes-risk-prediction)



#### Tools and Technologies



The project uses:



* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook
* Git and GitHub



#### Project Structure



diabetes-risk-analysis/

│

├── data/

│   ├── diabetes\_risk.csv

│   └── cleaned\_diabetes\_risk.csv

│

├── notebooks/

│   └── Week1\_Data\_Cleaning.ipynb

│

├── visualizations/

│   ├── bmi\_boxplot.png

│   └── fasting\_blood\_sugar\_boxplot.png

│

├── reports/

│   └── Week1\_Report.docx

│

└── README.md





#### Output



The cleaned dataset is saved as:



**cleaned\_diabetes\_risk.csv**



The notebook containing the data acquisition, exploration, cleaning, preprocessing, and validation steps is available in the 'notebooks' folder.



#### Future Work



The cleaned dataset will be used for further exploratory data analysis and visualization. This will include examining relationships between different variables, generating statistical summaries, creating visualizations, and identifying patterns related to diabetes risk.



Author: Aron P Jaison

