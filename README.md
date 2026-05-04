# silver-price-prediction
Integrating Machine Learning Models and Financial Analytics for Silver Price Prediction using ANN, RNN, and GRU
# 🥈 Silver Price Prediction using ANN, RNN, and GRU

> Forecasting silver prices using deep learning models on historical time series data.

---

## 📌 Project Overview

Silver is a highly volatile commodity influenced by market demand, economic conditions, and global factors. 
This project integrates financial analytics with deep learning to analyze historical silver price movements and forecast future prices using ANN, RNN, and GRU models.

---

## 🎯 Objectives

- Analyze historical silver price movements using time series data
- Identify candlestick patterns and technical trading indicators
- Build and train prediction models: ANN, RNN, and GRU
- Compare model performance to identify the most accurate approach

---

## 📊 Dataset

| Property   | Details                          |
|------------|----------------------------------|
| Source     | Yahoo Finance                    |
| Frequency  | Weekly data                      |
| Period     | 2000 – 2025                      |
| Features   | Date, Open, High, Low, Close, Volume |

---

## ⚙️ Data Preprocessing

- Handled missing values
- Extracted **candlestick patterns**:
  - Bullish Engulfing, Hammer, Shooting Star, Three Inside/Outside etc.,
- Computed **Technical Trading Ratios (TTR)**:
  - RSI, EMA, ATR, OBV, Aroon Oscillator, Parabolic SAR, Keltner Channel
- Applied **Min-Max Scaling** for feature normalization
- Split dataset into training and testing sets

---

## 🔍 Exploratory Data Analysis

- Visualized silver price trends over time
- Analyzed volatility and price fluctuations
- Studied candlestick behavior for market insights

---

## 🤖 Models Used

### 1. Artificial Neural Network (ANN)
Feedforward neural network that learns patterns using hidden layers and backpropagation.

### 2. Recurrent Neural Network (RNN)
Designed for sequential/time series data; leverages previous time steps for prediction.

### 3. Gated Recurrent Unit (GRU)
An advanced RNN variant that uses update and reset gates to better capture long-term dependencies.

---

## 🔁 Validation Method — Walk-Forward (Expanding Window)

This approach simulates real-world forecasting by progressively expanding the training set:
Train: Weeks 1–30  → Predict: Week 31
Train: Weeks 1–31  → Predict: Week 32
Train: Weeks 1–32  → Predict: Week 33
...and so on until the end of the dataset


---

## 📈 Model Evaluation

- Compared predicted vs. actual silver prices
- Evaluated using error metrics: **RMSE** and **MAE**
- Visualized predictions across the test period

---

## 🏆 Results

| Model | Performance        |
|-------|--------------------|
| GRU   | ✅ Best — lowest error, highest accuracy |
| RNN   | 🔶 Moderate performance |
| ANN   | 🔸 Comparatively lower accuracy |

**The GRU model outperformed the others**, owing to its ability to capture long-term dependencies in time series data.

---

## 📌 Conclusion

Among all models tested, **GRU is the most effective** for silver price prediction. Its gating mechanism allows it to retain relevant historical information over longer sequences, making it well-suited for financial time series forecasting.

---

## 🚀 Future Scope

- Implement **LSTM** for further comparison
- Incorporate macroeconomic indicators (inflation rate, USD index, etc.)
- Deploy the model via a **web-based dashboard**

---

## 👩‍💻 Author

**Santhini M**  
Feel free to connect or raise an issue for questions and suggestions!
