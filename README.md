# Demand-Forecasting-and-Inventory-Optimization
Demand forecasting and inventory optimization using time-series analysis and SARIMAX# 📊 Demand Forecasting and Inventory Optimization 

## 🎯 Project Overview
This project focuses on analyzing product demand patterns and optimizing inventory management using time series forecasting and inventory optimization techniques.

## 🔑 Key Components

### 1. 📥 Data Loading and Preprocessing
-  Imported necessary libraries (numpy, pandas, matplotlib, seaborn, plotly, statsmodels)
-  Loaded demand and inventory dataset
-  Cleaned data by removing unnecessary columns
-  Converted date column to datetime format

### 2. 📊 Data Visualization
-  Created interactive time series plots using Plotly:
  - **Demand Over Time**: Shows daily demand fluctuations
  - **Inventory Over Time**: Displays inventory depletion pattern

### 3. ⏰ Time Series Analysis
-  Performed differencing to make the time series stationary
-  Generated ACF (Autocorrelation Function) and PACF (Partial Autocorrelation Function) plots to identify seasonality and trends

### 4. 🔮 Demand Forecasting with SARIMAX
-  Implemented Seasonal ARIMA model with parameters:
  - Order: (1, 1, 1)
  - Seasonal Order: (1, 1, 1, 2) - accounting for 2-month seasonality
-  Generated 10-day demand forecasts

### 5. ⚖️ Inventory Optimization
Applied inventory management principles using:
- **Newsvendor Model** for optimal order quantity
- **Reorder Point** calculation
- **Safety Stock** determination
- **Total Cost** optimization considering:
  - Holding costs (10% of inventory value)
  - Stockout costs ($10 per unit)

## 📊 Key Results

### 🎯 Forecasted Demand (Next 10 days):
```
 2023-08-02: 117 units
 2023-08-03: 116 units
 2023-08-04: 130 units
 2023-08-05: 114 units
 2023-08-06: 128 units
 2023-08-07: 115 units
 2023-08-08: 129 units
 2023-08-09: 115 units
 2023-08-10: 129 units
 2023-08-11: 115 units
```

### 📦 Inventory Optimization Results:
- **Optimal Order Quantity**: 236 units
- **Reorder Point**: 235.25 units
- **Safety Stock**: 114.45 units
- **Total Cost**: $561.80

## 💼 Business Implications

1. **Demand Patterns**: The forecasting model captures seasonal fluctuations in product demand
2. **Inventory Strategy**: The optimized parameters help maintain adequate stock levels while minimizing costs
3. **Cost Efficiency**: The model balances holding costs against potential stockout costs
4. **Risk Management**: Safety stock provides buffer against demand variability

## 🔧 Technical Approach

- **Model Selection**: SARIMAX was chosen for its ability to handle both trend and seasonality
- **Parameter Tuning**: Seasonal parameters were set based on the 2-month data pattern
- **Validation**: Model performance could be further validated with additional historical data
- **Assumptions**: Lead time of 1 day and 95% service level were used as business parameters

## 🎉 Conclusion
This project demonstrates a complete pipeline from data analysis to actionable inventory management recommendations, providing a foundation for data-driven decision making in supply chain operations! 

## ⭐ **Show Your Support**

If you find this project helpful, please give it a **⭐ star** on GitHub!

---

***This project demonstrates the power of data analytics in supply chain optimization and inventory management efficiency.***
