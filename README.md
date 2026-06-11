# solar-power-generation-prediction
Solar Power Generation Prediction and Anomaly Detection using Machine Learning

# Solar Power Generation Prediction and Anomaly Detection

## About the Project

The objective of this project is to observe the extent to which machine learning can be integrated into solar energy systems. The provided dataset consists of battery status, load, and voltage and current readings from the solar system.

The primary objective of this project was to interpret the data, generate possible outcomes of solar power system generation, and analyze system behavior to identify abnormalities.



## What I Did

 1. Data Analysis

Data analysis was done through several steps:

- Identify and analyze missing values
- Eliminate unnecessary columns
- Encode categorical values to numerics
- Detect duplicates
- Enhance analysis using data visualizations

For this project, visualizations such as Correlation Heatmap, Boxplots, Battery Status Analysis, and Fault Analysis, were generated and analyzed.

---

2. Solar Power Generation Prediction

I used machine learning to predict existing solar panel current (pv_current).

**Model Used:** Random Forest Regressor

Steps Followed:

- Relevant features were selected
- Data was split into training and testing
- Model training was done
- Predictions were generated
- Model evaluation was done using MAE

**Result:**

MAE = approximately 0.03

The model accurately predicted solar current based on the data provided.

---
3. Anomaly Detection

The Isolation Forest algorithm was used to identify unusual records.

**Result:**

- Normal Records: 152
- Anomalies Detected: 8

These anomalies can be a sign of unexpected behavior from the system.

