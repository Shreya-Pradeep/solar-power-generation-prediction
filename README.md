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
## Setup Instructions

1. Download this repository.
2. Install the required Python libraries.

```bash
pip install pandas numpy matplotlib scikit-learn tensorflow joblib
```

3. Open the Jupyter notebooks.
4. Place the dataset in the project folder.
5. Run the notebooks one by one in order.
6. The trained model (.pkl) and TensorFlow Lite model (.tflite) will be generated after running the notebooks.
# Project Outputs

The project generated:

* Correlation Heatmaps
* Battery Status Analysis
* Fault Detection Visualizations
* Forecasting Results
* Prediction Outputs
* Anomaly Detection Results

---
## Approach Taken

The project was completed in the following steps:

- Loaded the solar monitoring dataset.
- Cleaned the data and handled missing values.
- Converted the timestamp into useful time features like hour and minute.
- Performed business insights to understand battery, solar and load behaviour.
- Built a forecasting model to predict PV current.
- Developed a TensorFlow model for prediction.
- Converted the trained model into TensorFlow Lite (.tflite) format for future deployment.

  ---
  ## Assumptions Made

- The dataset represents data collected from a solar monitoring system.
- The timestamp values are assumed to be correct.
- Missing values were handled during preprocessing.
- Since the current dataset contains only a short monitoring period, seasonal analysis is limited.
- The same workflow can be applied to larger datasets for better forecasting.

  ---

## Results Obtained

- Successfully cleaned and analysed the dataset.
- Generated business insights from battery, load and solar data.
- Built a forecasting model for PV current prediction.
- Trained a TensorFlow model.
- Converted the trained model into TensorFlow Lite (.tflite).
- Saved the trained machine learning model (.pkl).

  ---
  ## Business Insights Report

Some observations from the current dataset are:

- Average PV Current: 0.04 A
- Maximum PV Current: 3.8 A
- Average Battery Voltage: 14.25 V
- Most battery records were in the **Normal** state.
- The load remained mostly **OFF** during the available monitoring period.
- The current dataset is small, so long-term seasonal trends cannot be identified yet. These can be analysed when a larger dataset is available.

  ---
  ## Future Work

- Train the model using a larger historical dataset.
- Generate monthly and seasonal business insights.
- Improve forecasting accuracy.
- Use the TensorFlow Lite model for deployment on edge or mobile devices.

  ---

# Conclusion

This project demonstrates how Machine Learning techniques can be applied to solar energy systems for data analysis, business insights generation, forecasting, prediction, and anomaly detection. The combination of Random Forest and Isolation Forest provides valuable insights into solar system performance and supports data-driven decision making.

---

## Author

**Shreya P**

B.Tech Artificial Intelligence and Machine Learning
