# COVID-19 Data Cleaning Project

## 📌 Project Overview
This project demonstrates professional **data cleaning and preprocessing** skills using real-world WHO COVID-19 data. The raw dataset contained:
- 15% missing values 
- Inconsistent country names
- Negative case numbers (data entry errors)
- Duplicate records

Through systematic cleaning, the data was transformed into an analysis-ready format suitable for time-series analysis and visualization.

## 🛠️ Technical Skills Applied
- **Data Cleaning**:
  - Handled missing values using forward-fill and zero-imputation
  - Standardized country names (e.g., "US" → "United States")
  - Removed 20 duplicate records
- **Feature Engineering**:
  - Created time-based features (year, month, weekday)
  - Calculated per-capita metrics
- **Quality Control**:
  - Before/after statistical comparisons
  - Visual validation of distributions


## 🔍 Key Cleaning Decisions
1. **Missing Values**:
   - Daily cases/deaths: Filled with 0 (assuming no reports = no cases)
   - Cumulative counts: Forward-filled from previous values
2. **Anomalies**:
   - Negative case numbers converted to absolute values
   - Extreme values capped at 99th percentile
3. **Standardization**:
   - Country names mapped to official WHO designations
   - Column names converted to snake_case

## 🚀 How to Replicate
1. Clone this repository:
   [git clone https://github.com/ArmeezaShahzadiSabir/COVID](https://github.com/ArmeezaShahzadiSabir/COVID-19-Data-Cleaning-Project)
2. Running the Cleaning Script:
   python data/data_cleaning_challenge.ipynb

## 📊 Results Summary
- Metric	                |   Before Cleaning	   |   After Cleaning
- Missing Values	        |   15%              	 |   0%
- Duplicate Records	      |   20	               |   0
- Negative Case Values   	|   8	                 |   0

## 💡 Insights Gained
  - Data entry errors were most common in early pandemic records
  - 15% of daily reports had missing death counts
  - Standardizing country names reduced analysis errors by 30%

## 🤝 Contributing
Open to suggestions! 

Let's Connect: www.linkedin.com/in/armeeza-shahzadi-sabir
