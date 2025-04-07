# 📊 Medical Appointment No-Shows — Data Cleaning & Preprocessing

This project focuses on cleaning and preprocessing the **Medical Appointment No-Shows** dataset, which is commonly used for no-show prediction tasks in healthcare analytics.

## 🧾 Dataset Overview

The dataset includes over 110,000 medical appointment records from Brazil. It tracks whether a patient showed up for their appointment, along with other features like age, gender, and chronic conditions.

📁 [Source on Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments)

## ✅ Tasks Performed

Following standard data cleaning practices and steps mentioned in the project guide:

1. **Removed Duplicates**  
2. **Standardized Column Names**  
3. **Fixed Typos in Columns**  
   - `Hipertension` → `Hypertension`  
   - `Handcap` → `Handicap`
4. **Handled Data Types**  
   - Converted date columns to proper datetime format  
   - Ensured numeric and categorical columns were accurate
5. **Formatted Categorical Text**  
   - Cleaned the `No-show` column and converted to binary (`1 = No Show`, `0 = Show`)
6. **Converted Patient ID to String**  
7. **Created New Feature**  
   - `waiting_days`: Number of days between scheduling and appointment
8. **Reordered Columns Logically** for analysis

## 📂 Files Included

- `KaggleV2-May-2016.csv`: Original dataset (Kaggle)
- `Medical_Appointment_NoShows_Cleaned_Formatted.csv`: Final cleaned and formatted version
- `cleaning_script.py`: Python script used to clean and process the data
- `README.md`: Project documentation (this file)

## 🚀 How to Use

### Requirements
Make sure you have Python installed with the following packages:

pip install pandas

### 🧠 Conclusion
This project successfully demonstrates the importance of thorough data cleaning and preprocessing in real-world datasets. By standardizing the structure, correcting inconsistencies, and engineering useful features like waiting_days, the dataset is now ready for further exploration, visualization, and predictive modeling. Clean data not only enhances the quality of insights but also ensures more reliable outcomes in any downstream machine learning or statistical analysis.
