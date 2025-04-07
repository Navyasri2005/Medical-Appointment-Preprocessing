# 📊 Medical Appointment No-Shows — Data Cleaning & Preprocessing

This project focuses on cleaning and preprocessing the **Medical Appointment No-Shows** dataset, which is commonly used for no-show prediction tasks in healthcare analytics.

## 🧾 Dataset Overview

The dataset includes over 110,000 medical appointment records from Brazil. It tracks whether a patient showed up for their appointment, along with other features like age, gender, and chronic conditions.

📁 [Dataset Source on Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments)

## ✅ Tasks Performed

The following cleaning and preprocessing tasks were applied:

1. **Removed Duplicates**  
2. **Standardized Column Names**  
3. **Corrected Typos**  
   - `Hipertension` → `Hypertension`  
   - `Handcap` → `Handicap`
4. **Handled Data Types**  
   - Converted `scheduledday` and `appointmentday` to datetime format  
   - Ensured `age`, `handicap`, and flags were in the correct format
5. **Standardized Categorical Text**  
   - Cleaned and binarized `no_show` column (`0 = Show`, `1 = No Show`)
6. **Converted `patientid` to String**  
   - Prevents formatting issues with large numerical IDs
7. **Created New Feature**  
   - `waiting_days`: Days between scheduling and appointment
8. **Reordered Columns**  
   - Grouped logically by patient, appointment, conditions, and outcome

## 📂 Files Included

- `KaggleV2-May-2016.csv`: Original dataset from Kaggle
- `Medical_Appointment_NoShows_Cleaned_Formatted.csv`: Cleaned and final version
- `cleaning_script.py`: Python script that performs all the cleaning steps
- `README.md`: Project documentation

## 🚀 How to Use

### Requirements
Make sure you have Python installed with the following package:
```bash
pip install pandas
```

### 🧠 Conclusion
---
This project successfully demonstrates the importance of thorough data cleaning and preprocessing in real-world datasets. By standardizing the structure, correcting inconsistencies, and engineering useful features like `waiting_days`, the dataset is now ready for further exploration, visualization, and predictive modeling. Clean data not only enhances the quality of insights but also ensures more reliable outcomes in any downstream machine learning or statistical analysis.

### Run the Script
To generate the cleaned dataset:
```bash
python cleaning_script.py
```

This will output:  
📄 `Medical_Appointment_NoShows_Cleaned_Formatted.csv`

---

Feel free to fork or clone this repo and build upon it for your own data analysis or machine learning projects!




