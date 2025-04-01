📈 Stock Price Prediction and Correlation Analysis Using LSTM
Contributors:
Shreeya Yashvi (055045)
Kashish Srivastava (055046)
🎯 Objective
The goal of this project is to develop a Long Short-Term Memory (LSTM) model to predict stock prices of NIFTY 50 and TCS (Tata Consultancy Services). Additionally, the project analyzes the impact of TCS stock movements on the NIFTY 50 index.

📝 Problem Statement
Can we accurately predict future stock prices using historical data?
What is the degree of correlation between NIFTY 50 and TCS stock movements?
How well does the LSTM model capture trends and volatility in stock prices?
📚 Dataset
NIFTY 50 Index: Ticker ^NSEI (National Stock Exchange Index)
TCS Stock: Ticker TCS.NS
Date Range: Historical stock prices from 2005-01-31 to 2025-01-31 fetched using yfinance library.
⚙️ Model Architecture
1. Input Layer
Sequence length: 60 days
Feature: Closing prices
2. LSTM Layers
3 LSTM layers with 50 units each
Dropout (0.2) applied after each LSTM layer to prevent overfitting
3. Dense Layers
1 Dense layer with 25 units and ReLU activation
1 Output layer with 1 neuron (predicts the next day’s closing price)
🔥 Model Training
Train-Test Split: 80% for training, 20% for testing
Loss Function: Mean Squared Error (MSE)
Optimizer: Adam (learning rate = 0.001)
Epochs: 10
📊 Results & Observations
NIFTY 50 Accuracy: Achieved ~95.36% accuracy in predicting NIFTY 50 prices.
TCS Accuracy: Attained ~95.59% accuracy in predicting TCS stock prices.
Strong positive correlation between NIFTY 50 and TCS stock prices.
Model captures long-term trends effectively but underperforms during high volatility periods.
💡 Managerial Insights
Investment Decisions: Enables better decision-making by forecasting future trends.
Market Behavior Analysis: Provides insights into the impact of blue-chip stocks like TCS on the broader market.
Model Limitations: Does not account for macroeconomic factors or market sentiment.
🚀 Future Enhancements
Incorporate technical indicators (RSI, MACD, Bollinger Bands).
Explore transformer-based models for improved accuracy.
Integrate sentiment analysis from news and social media.
