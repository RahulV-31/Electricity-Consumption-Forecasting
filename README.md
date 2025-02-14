**1. Electricity Consumption Forecasting**

---

**Project Overview**  
This project aims to:  
- Predict electricity demand using historical consumption data and weather conditions.  
- Enable effective energy management by reducing wastage and ensuring grid stability.

---

**Dataset**  
- **Electricity Data**: Records of electricity demand and day-ahead demand forecasts.  
- **Weather Data**: Includes temperature, humidity, wind speed, dew point, and other weather-related variables.  
- Merged both datasets on a common timestamp for alignment.  

---

**Objective**  
The project goals include:  
- Exploring and preprocessing the datasets for analysis.  
- Engineering features to capture temporal and weather patterns.  
- Building and evaluating a machine learning model for electricity demand forecasting.  
- Providing actionable insights for better energy management.  

---

**Project Workflow**  
1. Data Collection and Loading:  
   - Merged electricity demand and weather data into a single dataset.  

2. Data Preprocessing:  
   - Removed irrelevant columns and handled missing values.  
   - Tested two approaches for handling missing data:  
     - Dropping rows with missing values.  
     - Imputing missing values using mean/mode for numerical and categorical features.  

3. Feature Engineering:  
   - Extracted temporal features such as year, month, day, day of the week, and weekend indicators.  
   - Selected key weather variables (e.g., temperature, humidity, wind speed) for analysis.  

4. Exploratory Data Analysis (EDA):  
   - Visualized electricity demand trends over time.  
   - Analyzed correlations between features and electricity demand using heatmaps.  

5. Modeling:  
   - Implemented a Random Forest Regressor for forecasting.  
   - Split data into training and testing sets (80-20 split).  

6. Evaluation:  
   - Assessed model performance using:  
     - RMSE (Root Mean Square Error).  
     - MAE (Mean Absolute Error).  
     - R² Score.

---

**Results**
- Method 1 (Dropping Null Values):  
  - RMSE: 6,196.02  
  - MAE: 3,887.18  
  - R² Score: 0.79  
- Method 2 (Imputing Null Values):  
  - RMSE: 7,542.66  
  - MAE: 4,504.52  
  - R² Score: 0.65  
- Dropping rows with missing values yielded better performance, highlighting the importance of data quality.  

---

**Tools and Technologies**
- Programming Language: Python  
- Libraries:  
  - Data Analysis: Pandas, NumPy  
  - Visualization: Matplotlib, Seaborn  
  - Machine Learning: scikit-learn  

---

Colab Notebook

   Explore the full implementation of this project in the [Colab Notebook](https://colab.research.google.com/drive/1k4mq1GoxqfHP9u5bVxv2W0Gegzd3QbBm?usp=sharing).
