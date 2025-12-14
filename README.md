# COVID-19 Clinical Trials – Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project performs **Exploratory Data Analysis (EDA)** on COVID-19 clinical trial data obtained from **ClinicalTrials.gov**, a publicly available database maintained by the U.S. National Library of Medicine.

The goal of this project is to **clean, analyze, and visualize** real-world clinical trial data to understand:
- Trial distribution across countries
- Current status of trials
- Gender eligibility
- Enrollment patterns
- Trends over time

This project demonstrates practical **data cleaning, feature engineering, missing value handling, and visualization skills** using Python.

---

## 🎯 Objectives
- Understand the structure and quality of clinical trial data
- Handle missing and inconsistent data logically
- Extract useful features from raw text data
- Generate meaningful visual insights
- Prepare a clean dataset for further analysis or modeling

---

## 🛠️ Tools & Technologies Used
- **Python**
- **Pandas** – Data manipulation
- **NumPy** – Numerical operations
- **Matplotlib & Seaborn** – Data visualization
- **Jupyter Notebook / Python Script**

---

## 📂 Dataset Information
- **Source:** ClinicalTrials.gov  
- **Dataset Name:** COVID clinical trials.csv  
- **Records:** ~5,700 clinical trials  
- **Features:** Trial status, phase, gender, enrollment, locations, dates, etc.

The dataset contains real-world challenges such as missing values, text-heavy fields, and skewed numerical data.

---

## 🔍 Project Workflow

### 1️⃣ Data Loading & Inspection
- Loaded CSV dataset using Pandas
- Inspected shape, columns, and data types
- Identified categorical and numerical features

### 2️⃣ Missing Data Analysis
- Calculated missing value percentages
- Dropped columns with extremely high missing data:
  - `Results First Posted`
  - `Study Documents`

### 3️⃣ Data Cleaning
- Removed duplicate records
- Ensured minimum data quality by threshold filtering
- Classified missing data patterns (MAR)

### 4️⃣ Feature Engineering
- Extracted **Country** information from the `Locations` column
- Created a new `Country` feature for geographical analysis

### 5️⃣ Missing Value Handling
- Categorical columns filled with `"Missing <column_name>"`
- Numerical column (`Enrollment`) filled using **median imputation** due to high skewness

### 6️⃣ Data Visualization
Generated and saved the following visualizations:
- Top 10 countries conducting COVID-19 trials
- Distribution of trial status
- Gender eligibility distribution
- Trial start month distribution
- Missing data percentage by feature

### 7️⃣ Output Generation
- Saved cleaned dataset as CSV
- Saved all plots as PNG files
- Saved full Python script automatically

---

## 📊 Key Insights
- The **United States** has the highest number of COVID-19 clinical trials
- Most trials are either **Recruiting** or **Completed**
- Majority of trials are open to **all genders**
- Enrollment data is highly skewed, indicating a few very large studies
- Trial activity peaked during early pandemic months

---

## 📁 Project Structure
