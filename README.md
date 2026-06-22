# Solar Power Generation Prediction, Forecasting and Anomaly Detection

## Project Overview

This project focuses on analyzing solar energy system data, generating business insights, forecasting solar power generation, and detecting anomalies using Machine Learning.

The dataset contains battery status, battery voltage and current, load parameters, solar panel measurements, and system performance indicators. The objective is to understand system behavior, generate insights, predict solar power generation, and identify abnormal conditions that may affect efficiency.

---

## Objectives

* Perform data cleaning and preprocessing
* Generate business insights from solar system data
* Analyze battery and solar panel performance
* Predict solar power generation using Machine Learning
* Forecast future solar generation values
* Detect anomalies and unusual system behavior
* Visualize trends and relationships in the data

---

## Dataset Features

The dataset contains parameters such as:

* Battery Current (`bat_current`)
* Battery Voltage (`bat_volt`)
* Battery Status (`bat_status`)
* Load Current (`load_current`)
* Load Voltage (`load_volt`)
* Solar Panel Current (`pv_current`)
* Solar Panel Voltage (`pv_volt`)
* State of Charge (`soc`)
* Depth of Discharge (`dod`)
* Timestamp Information (`metadata_date`)

---

# 1. Data Analysis and Preprocessing

Several preprocessing steps were performed before model building.

### Data Cleaning

* Identified missing values
* Removed unnecessary columns
* Checked and removed duplicate records
* Handled inconsistent data entries
* Converted categorical variables into numerical format

### Exploratory Data Analysis (EDA)

The following visualizations were generated:

* Correlation Heatmap
* Boxplots
* Battery Status Analysis
* Fault Analysis
* Solar Panel Performance Analysis
* Voltage and Current Distribution Analysis

These visualizations helped understand system behavior and identify important relationships between variables.

---

# 2. Business Insights

Business insights were generated from the dataset to understand the overall performance and efficiency of the solar energy system.

### Key Insights

* Battery voltage remained stable during normal operation.
* Solar panel current varied according to system conditions.
* Load consumption patterns were identified through current and voltage analysis.
* Battery status provided insights into charging and discharging behavior.
* Correlation analysis revealed relationships among battery, load, and solar parameters.

### Benefits

* Better monitoring of solar system performance
* Improved operational efficiency
* Data-driven decision making
* Early identification of performance issues

---

# 3. Solar Power Generation Prediction

Machine Learning was used to predict solar panel current (`pv_current`).

### Model Used

**Random Forest Regressor**

### Steps Followed

* Feature Selection
* Train-Test Split
* Model Training
* Prediction Generation
* Model Evaluation

### Result

* Mean Absolute Error (MAE): ~0.03

The model accurately predicted solar current using system parameters.

---

# 4. Solar Power Forecasting

A forecasting model was developed and saved as a `.pkl` file for future predictions.

### Forecasting Process

* Historical solar system data was analyzed
* Relevant features were selected
* Machine learning model was trained
* Future values were predicted
* Model was saved using Pickle (`.pkl`) for deployment and reuse

### Outcome

The forecasting model can be loaded and used to predict future solar power generation values based on system parameters.

---

# 5. Anomaly Detection

The Isolation Forest algorithm was used to identify unusual observations within the dataset.

### Model Used

**Isolation Forest**

### Results

* Normal Records: 152
* Anomalies Detected: 8

These anomalies may indicate unexpected behavior, sensor issues, or potential system faults.

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Pickle (.pkl)
* Jupyter Notebook

---

# Project Outputs

The project generated:

* Correlation Heatmaps
* Battery Status Analysis
* Fault Detection Visualizations
* Forecasting Results
* Prediction Outputs
* Anomaly Detection Results

---

# Conclusion

This project demonstrates how Machine Learning techniques can be applied to solar energy systems for data analysis, business insights generation, forecasting, prediction, and anomaly detection. The combination of Random Forest and Isolation Forest provides valuable insights into solar system performance and supports data-driven decision making.

---

## Author

**Shreya P**

B.Tech Artificial Intelligence and Machine Learning
