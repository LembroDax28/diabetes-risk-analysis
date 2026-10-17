# Diabetes Risk Analysis

This project is part of my internship work in data analysis. It focuses on working with a diabetes risk dataset and performing data acquisition, exploration, cleaning, preprocessing, exploratory data analysis (EDA), and visualization.

## Project Overview

The dataset contains information about patients, including demographic details, lifestyle factors, and health-related measurements. The objective is to examine data quality, prepare the dataset for analysis, and explore patterns and relationships between health and lifestyle variables and diabetes risk categories.

## Week 1 — Data Cleaning and Preprocessing

The first week of the project focused on:

- Acquiring a public diabetes risk dataset
- Understanding the structure and contents of the dataset
- Checking data types and categorical values
- Identifying missing values
- Checking for duplicate records
- Verifying patient IDs
- Detecting potential numerical outliers using the IQR method
- Investigating potential outliers using box plots
- Handling missing categorical values
- Validating the cleaned dataset
- Exporting the cleaned dataset for further analysis

### Missing Value Handling

Missing values were found in the following categorical columns:

- `smoking_status`
- `alcohol_consumption`
- `income_bracket`

These missing values were replaced with `Unknown` so that the records could be retained without introducing assumptions about the missing information.

### Outlier Detection

Potential numerical outliers were identified using the **Interquartile Range (IQR)** method.

The following numerical variables were examined:

- Age
- BMI
- Hours of sleep per night
- Stress level
- Fasting blood sugar
- HbA1c level
- Systolic blood pressure
- Diastolic blood pressure
- Waist circumference

Potential outliers were investigated using box plots, particularly for BMI and fasting blood sugar. The detected values were not automatically removed because unusual health measurements may represent valid observations rather than erroneous data.

### Week 1 Deliverables

- **Notebook:** `notebooks/Week1_Data_Cleaning.ipynb`
- **Report:** `reports/Week_1.docx`
- **Cleaned dataset:** `data/cleaned_diabetes_risk.csv`

## Week 2 — Exploratory Data Analysis and Visualization

The second week focused on exploring the cleaned dataset using Python libraries and visualizing patterns in the data.

The work included:

- Analyzing the distribution of diabetes risk categories
- Examining the distribution of patient ages
- Comparing BMI across diabetes risk categories
- Comparing average HbA1c levels across diabetes risk categories
- Exploring correlations among numerical variables
- Investigating diabetes risk distributions by family history of diabetes
- Examining diabetes risk distributions by physical activity level
- Comparing fasting blood sugar across diabetes risk categories
- Exploring sleep duration across diabetes risk categories
- Generating statistical summaries and visualizations
- Documenting key findings and limitations

### Week 2 Deliverables

- **Notebook:** `notebooks/Week2_EDA.ipynb`
- **Report:** `reports/Week_2.docx`
- **Visualizations:** `visualizations/Week_2/`

## Dataset

The dataset contains **15,000 records and 19 columns**.

Some of the main variables include:

- `patient_id`
- `age`
- `gender`
- `city`
- `bmi`
- `family_history_diabetes`
- `physical_activity_level`
- `diet_type`
- `smoking_status`
- `alcohol_consumption`
- `hours_sleep_per_night`
- `stress_level`
- `fasting_blood_sugar`
- `hba1c_level`
- `blood_pressure_systolic`
- `blood_pressure_diastolic`
- `waist_circumference_cm`
- `income_bracket`
- `diabetes_risk`

**Dataset source:** [Diabetes Risk Prediction Dataset — Kaggle](https://www.kaggle.com/datasets/mansiaggarwal88/diabetes-risk-prediction)

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Git
- GitHub

## Project Structure

```text
diabetes-risk-analysis/
├── data/
│   ├── diabetes_risk.csv
│   └── cleaned_diabetes_risk.csv
├── notebooks/
│   ├── Week1_Data_Cleaning.ipynb
│   └── Week2_EDA.ipynb
├── visualizations/
│   ├── Week_1/
│   └── Week_2/
├── reports/
│   ├── Week_1.docx
│   └── Week_2.docx
└── README.md
```

## Key Findings

The exploratory data analysis revealed several patterns in the dataset:

- BMI and waist circumference showed a strong positive correlation.
- Fasting blood sugar and HbA1c levels showed a strong positive correlation.
- The distribution of diabetes risk categories differed across family-history groups.
- Higher physical activity levels were associated with a lower proportion of high-risk records in this dataset.
- Sleep duration was broadly similar across the diabetes risk categories.

These findings describe associations and patterns within the dataset. They do not establish causation or provide medical diagnoses.

## How to Run the Project

1. Clone or download the repository.
2. Install the required Python libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. Open a terminal in the project directory.
4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open the required notebook from the `notebooks/` folder and run its cells in order.

The notebooks use relative paths to access the dataset, so keep the project folder structure intact.

## Future Work

Future work may include deeper statistical analysis, feature engineering, and further investigation of relationships between health measurements, lifestyle factors, and diabetes risk. Additional analysis could also explore predictive modeling, subject to the dataset's suitability and limitations.

## Disclaimer

This project is intended for educational purposes and exploratory data analysis only. Its findings should not be used for clinical diagnosis or medical decision-making.

**Author:** Aron P Jaison