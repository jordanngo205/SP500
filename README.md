# SP500

# Stock Market Prediction Using Machine Learning

## 📌 Overview
This project applies **machine learning techniques** to predict stock price movements based on historical market data. It leverages technical indicators and **Random Forest & LSTM models** to forecast whether a stock will close higher or lower the next day.

## 🚀 Features
- Fetches historical stock data using **Yahoo Finance (yfinance)**.
- Implements **feature engineering** (SMA, EMA, MACD, Volatility, RSI, Bollinger Bands, etc.).
- Uses **Random Forest Classifier** and **LSTM** for predictive modeling.
- Evaluates model performance with **accuracy score & classification report**.
- Predicts the next day’s stock movement for multiple stocks (SPY, JNJ, PG, etc.).


## 📊 Data Collection
The project uses **Yahoo Finance API** (`yfinance`) to fetch historical stock prices for:
- `S&P 500 (^GSPC)`
- `Johnson & Johnson (JNJ)`
- `Procter & Gamble (PG)`
- `Coca-Cola (KO)`
- `Microsoft (MSFT)`
- `SPDR S&P 500 ETF Trust (SPY)`
- `Vanguard Dividend Appreciation ETF (VIG)`
- `Health Care Select Sector SPDR Fund (XLV)`

## 📈 Machine Learning Models
### 🔹 **Random Forest Classifier**
- Uses 200 trees (`n_estimators=200`), max depth of 5.
- Predicts whether the stock will go **UP 📈** or **DOWN 📉** based on past trends.

### 🔹 **Long Short-Term Memory (LSTM) Neural Network**
- Trained with `50 units`, `Dropout=0.2`, and `epochs=20`.
- Sequences data over a **10-day window** for pattern recognition.

## 📊 Evaluation Metrics
- **Accuracy Score** (`accuracy_score` from scikit-learn)
- **Precision, Recall, F1-score** (via `classification_report`)

## 📢 Results
- The **Random Forest model** achieves an accuracy of **~60%-70%**, varying by stock.
- The **LSTM model** captures sequential patterns but requires fine-tuning for stability.
- Predictions are stored in a Pandas DataFrame and printed as a summary table.

## 🔮 Future Improvements
- **Feature Expansion:** Incorporate more technical indicators (e.g., Fibonacci Retracement, VWAP, etc.).
- **Hyperparameter Tuning:** Optimize model parameters for better predictive accuracy.
- **Ensemble Methods:** Combine Random Forest and LSTM for robust predictions.
- **Live Trading Integration:** Connect with an API like Alpaca for real-time execution.

## 📜 License
This project is licensed under the **MIT License**.

---
🚀 **Contributions & Feedback** are welcome! If you have suggestions or improvements, feel free to open an issue or pull request. Happy coding! 🎯

