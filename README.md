# ⚡ Energy Consumption Forecasting (ARIMA vs Random Forest)

##  Project Overview
This project focuses on forecasting household energy consumption using both **Time Series modeling (ARIMA)** and **Machine Learning (Random Forest)**.

The goal is to compare traditional statistical methods with modern ML approaches.

---

##  Objectives
- Clean and preprocess time series data
- Perform time-based feature engineering
- Apply ARIMA for forecasting
- Apply Random Forest for regression-based prediction
- Compare model performance

---

##  Dataset
- Dataset: Household Power Consumption Dataset
- Features used:
  - Date & Time
  - Global Active Power (target variable)

---

##  Technologies Used
- Python 🐍
- Pandas & NumPy
- Matplotlib
- Scikit-learn
- Statsmodels

---

##  Workflow

### 1️ Data Preprocessing
- Combined Date & Time into Datetime
- Converted power consumption to numeric
- Removed missing values
- Set Datetime as index

### 2️⃣ Time Series Resampling
- Resampled data to hourly frequency
- Aggregated using mean values

### 3️⃣ Feature Engineering
- Extracted:
  - Hour
  - Day of Week
  - Weekend indicator

### 4️⃣ Model Building

#### 📈 ARIMA Model
- Used ARIMA(5,1,0)
- Captures temporal dependencies

#### 🌲 Random Forest
- Used time-based features
- Handles non-linear relationships

---

## 📈 Model Evaluation
Metrics used:
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)

Both models were evaluated on unseen test data.

---

##  Visualization
- Actual vs Predicted values
- ARIMA vs Random Forest comparison

---

##  Key Learnings
- Difference between Time Series and ML approaches
- Importance of datetime feature engineering
- Model comparison for better forecasting
- Handling real-world noisy data

---

##  Future Improvements
- Hyperparameter tuning (ARIMA & RF)
- Use advanced models (LSTM, Prophet, XGBoost)
- Add seasonality analysis
- Deploy forecasting dashboard using Streamlit

---

## 🔗 How to Run

```bash
git clone https://github.com/your-username/energy-forecasting.git
cd energy-forecasting
pip install -r requirements.txt
python main.py
