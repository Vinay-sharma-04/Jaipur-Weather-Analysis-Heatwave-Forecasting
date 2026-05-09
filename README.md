# 🌡️ Heatwave Prediction and Temperature Forecasting

## 📌 Overview

This project focuses on analyzing historical weather data and building Machine Learning models for:

* Heatwave Prediction (Classification)
* Next-Day Temperature Forecasting (Regression)

The project uses historical weather data from the Open-Meteo API and applies different Machine Learning techniques using Python and Scikit-learn.

---

## 🚀 Features

✔️ Data Cleaning and Preprocessing
✔️ Feature Engineering using Lag Features & Rolling Averages
✔️ Heatwave Detection and Prediction
✔️ Next-Day Temperature Forecasting
✔️ Data Visualization and Trend Analysis
✔️ Model Training and Evaluation
✔️ Model Saving using Joblib

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Joblib

---

## 📂 Dataset

The dataset contains historical weather information such as:

* Maximum Temperature
* Humidity
* Wind Speed
* Precipitation
* Weather Conditions

### Data Source

Open-Meteo API

---

## 🤖 Machine Learning Models

### 🔥 Heatwave Prediction

A heatwave day is defined as:

```python
Temperature >= 40°C
```

#### Models Used

* Logistic Regression
* Random Forest Classifier

#### Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

### 🌤️ Temperature Forecasting

This project also predicts the next day's maximum temperature.

#### Models Used

* Linear Regression
* Random Forest Regressor

#### Evaluation Metrics

* MAE
* RMSE
* R² Score

---

## 📊 Visualizations

The project includes:

* Monthly Heatwave Analysis
* Yearly Heatwave Trends
* Feature Importance Graphs
* Actual vs Predicted Temperature Plot
* Error Distribution Analysis

---

## 📁 Project Structure

```bash
├── Model(2).ipynb
├── dataset.csv
├── heatwave_model.pkl
├── temperature_model.pkl
└── README.md
```

---

## 🔄 Workflow

1. Data Collection
2. Data Cleaning
3. Feature Engineering
4. Train-Test Split
5. Model Training
6. Model Evaluation
7. Visualization
8. Model Saving

---

## 🌱 Future Improvements

* Add Deep Learning models like LSTM
* Deploy using Streamlit or Flask
* Add Real-Time Weather Forecasting
