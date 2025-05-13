# 📈 Stock Price Prediction Analysis

📎 Rachel Kim, K***  
📅 Date: 2025.04  
📚 Team Project (2p)  


📝 This project aims to predict stock prices using QQQ stock dataset. The analysis includes data loading, EDA, feature engineering, and applying machine learning models to predict future stock prices.


    
## 📂 Project Overview
The project includes the following steps:  
•	Data Loading: Obtaining stock data from yahoo finance API.  
•	Exploratory Data Analysis (EDA): Visualizing trends, patterns, seasonality in the data.  
•	Feature Engineering (Technical Indicators) : Adding technical indicators (e.g. MA5, RSI...)  
•	Modeling (1): Building models to predict future stock prices with existing data and added technical indicators.  
•	Feature Engineering (Economical Indicators) : Adding economical indicators (e.g. insterest, gold price, CPI) for a more detailed analysis.  
•	Modeling (2): Building enhanced models to predict future stock prices with added economical indicators.  
•	Model Evaluation: Evaluating the performance of the models using MAE and accuracy score.  



## 📂 Requirements  
To run the code and replicate the analysis, we used the following Python libraries:  
•	pandas: Data manipulation and analysis.  
•	numpy: Numerical operations.  
•	matplotlib: Plotting and data visualization.  
•	seaborn: Statistical data visualization.  
•	scikit-learn: Machine learning models and utilities.  
•	tensorflow: Deep learning framework (for LSTM models).  
•	keras: Deep learning framework (for LSTM models).  
•	datetime: Working with date and time.  
•	yfinance: Yahoo Finance API (if using stock data).  

## 📂 Files in the folder  
•	**QQQ Stock Price Prediction.ipynb**: Jupyter Notebook containing the complete analysis.    
•	**QQQ Presentation.pdf**: Presentation file    
•	**datasets**: Folder containing our datasets   
QQQ (200101-241231) : Original Dataset   
QQQ_tech(200101-241231) : Original + tech indicators dataset   
QQQ_tech, macro(200101-241231) : Original + tech + economical dataset  
•	**Read me** : Descriptions of the process and summary  





## 📂 Results  
**Model MAE**  

<img width="527" alt="image" src="https://github.com/user-attachments/assets/1ef36030-895c-45b8-91b7-2ba7a26f1dce" />  


**Accuracy**  
<img width="452" alt="image" src="https://github.com/user-attachments/assets/0171a2be-274b-4dc8-92c4-ff833e1648b2" />  

 
This bar chart compares the accuracy of different models within a ±1% error margin. The Linear Regression (Tech + Macro) model achieved the highest accuracy at 78.10%, followed by Linear Regression (Tech Only) and XGBoost (Tech + Macro). 
In contrast, both LSTM models showed the same low accuracy (5.76%), suggesting that LSTM struggled to learn effectively from the data; possibly due to insufficient training time, model complexity, or the short sequence length used for time series input.  

## 📂 Key Takeaways  

QQQ analytics project demonstrated that combining technical indicators with macroeconomic features (external features) significantly improves the accuracy of traditional machine learning models like Linear Regression and XGBoost for stock price prediction.   
Among all approaches, Linear Regression with both technical and macro data delivered the highest accuracy, proving that simplicity, when paired with meaningful features, can outperform more complex models like LSTM. This highlights the importance of thoughtful feature engineering and model selection over relying solely on deep learning architectures.  

## 📂 References  
QQQ Historical Stock Data (2020–2024) was retrieved using the yfinance Python library.  
Source: Yahoo Finance, via yfinance package.  
Ticker: "QQQ" — Invesco QQQ Trust  

“Stock Market Analysis + Prediction Using LSTM.” Kaggle.com,  
www.kaggle.com/code/faressayah/stock-market-analysis-prediction-using-lstm  

“LSTM Time Series + Stock Price Prediction = FAIL.” Kaggle.com,   
www.kaggle.com/code/carlmcbrideellis/lstm-time-series-stock-price-prediction-fail  

“Stock Price Prediction Using XGBOOST PROPHET ARIMA.” Kaggle.com, Kaggle, 15 Mar. 2024,   
www.kaggle.com/code/zeyadsayedadbullah/stock-price-prediction-using-xgboost-prophet-arima  

