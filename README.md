
# 📈 **Microsoft Stock Price Forecasting Using Time Series Analysis**

This project aims to forecast the future movements of **Microsoft's stock prices (MSFT)** using advanced **time series analysis** techniques. The key focus is on predicting the **day-to-day changes in closing prices** (`close_diff`), which provides valuable insights into **price momentum, volatility, and market trends**.

## 🔍 **Research Question** 
**Can time series models like ARIMA and LSTM accurately predict Microsoft (MSFT) stock prices, and what insights do they offer for financial decision-making?**

## 📊 **Key Targets**
- **Target Variable**: **`close_diff`** – Daily change in stock's closing price
- **Predicted Outputs**:  
    - **30-day Price Forecasts**  
    - **Volatility Clusters**  
    - **Trend Classifications**  

## 🧠 **Models Used**
- **ARIMA**: Traditional time series forecasting model
- **SARIMA**: Enhanced ARIMA with seasonal components
- **SARIMAX**: SARIMA with exogenous variables
- **LSTM**: Deep learning model for capturing complex temporal patterns

## 🛠️ **Tools & Libraries**
- **Python** 🐍
- **Pandas** 📊
- **Numpy** 🔢
- **Matplotlib** and **Seaborn** 📈
- **Statsmodels** (ARIMA, SARIMA, SARIMAX) 📉
- **TensorFlow** (LSTM) 🤖
- **Scikit-learn** 🔧

## 📉 **Final Results**
The **SARIMAX model** outperformed all other tested variants in predicting MSFT stock prices, achieving the following metrics:
- **Training MAE**: 0.3048
- **Testing MAE**: 1.2192
- **Training RMSE**: 0.4279
- **Testing RMSE**: 1.6700
- **MAPE (Training)**: 0.0038
- **MAPE (Testing)**: 0.0064

**SARIMAX** proved to be the most accurate due to its ability to incorporate both **seasonal components** and **exogenous variables**, making it ideal for stock price prediction.

## 🔄 **Flow of the Project**
1. **Data Collection**: Gathered historical MSFT stock data (2010–2023) including OHLC prices, volume, and moving averages.  
2. **Preprocessing**: Cleaned and normalized data, handling missing values and outliers.  
3. **Feature Engineering**: Created relevant features like moving averages, price momentum, and volatility indicators.  
4. **Model Training & Evaluation**: Trained ARIMA, SARIMA, SARIMAX, and LSTM models, evaluating them using **MAE, RMSE, and MAPE** metrics.  
5. **Forecasting & Analysis**: Generated 30-day price forecasts, identified volatility clusters, and categorized trends.  
6. **Conclusion**: Provided recommendations for stock prediction based on the performance of each model.

## 🚀 **Usage**
Clone this repo and run the notebook to reproduce the stock price forecasting process and evaluate the models.  
```bash
git clone https://github.com/yourusername/microsoft-stock-forecasting.git
cd microsoft-stock-forecasting
jupyter notebook
