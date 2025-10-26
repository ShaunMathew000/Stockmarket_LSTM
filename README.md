# Stock Market Prediction

## 🌿 **Project Overview**  
Built an LSTM-based forecasting model in TensorFlow. Conducted EDA and engineered time-of-day features on intraday stock data from Tata Motors.

- Data cleaning and preprocessing of minute-level stock data (Tata Motors)
- Extraction of time-based features
- Visualization of price and volume trends by hour and session
- Feature selection using Lasso regression
- Cyclic time encoding for ML compatibility
- Predictive modeling using deep learning (LSTM neural network)


## 💻 Model Architecture

### Data Upload and Preprocessing

Uploaded the minute-level CSV dataset (TataMotors.csv)
Filled missing values via forward fill to maintain time-series continuity
Converted date columns to proper datetime format

### Feature Engineering

Extracted Hour and DayOfWeek from timestamps
Analyzes closing prices and volumes by hour and session (morning/afternoon)

### Visualization

Line and bar plots for hourly price/volume trends
Comparison bar plots for morning vs. afternoon price and volume

### Cyclic Time Encoding

Encode hours cyclically (Hour_sin, Hour_cos) to preserve temporal relationships

### Feature Selection

Apply Lasso regression to select impactful features for prediction
Use cyclically encoded hour features and key technical indicators (Open, High, Low, Close, Volume)

### LSTM Model Training

Prepare data using a rolling window (sequence length)
Build and train an LSTM neural network model
Evaluate using RMSE and MAE
Compare predicted and actual closing prices with visualizations


## 📈 Performance and Results

- Peak trading hours identified using hourly aggregation and trend plots

- Morning and afternoon session analysis highlights temporal market behaviors

- Lasso regression highlights the most impactful predictive features

- LSTM model demonstrates ability to predict closing prices with reasonable accuracy, shown via RMSE/MAE and prediction plots

  <img width="933" height="701" alt="image" src="https://github.com/user-attachments/assets/87017541-1670-4e82-a19e-4f2953d4a43e" />


  <img width="916" height="701" alt="image" src="https://github.com/user-attachments/assets/29585da4-afd4-4be0-8783-a64be61bcd34" />


 <img width="185" height="70" alt="image" src="https://github.com/user-attachments/assets/2a49ed2e-0a6d-40b6-8b0a-fd048c5ef26b" />


  <img width="988" height="547" alt="image" src="https://github.com/user-attachments/assets/127a5f1f-1ca4-4877-9de5-86778d5f75f9" />


  <img width="708" height="547" alt="image" src="https://github.com/user-attachments/assets/487a0fe4-8cd6-4aad-b6ed-554cbee143b1" />

  
---

## 🚀 Getting Started

To run this model locally , download and run the StockMarket_LSTM_ToD.ipynb file in the repository.


