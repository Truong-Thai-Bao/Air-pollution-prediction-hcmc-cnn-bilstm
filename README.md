# Air Pollution Prediction in Ho Chi Minh City using CNN-BiLSTM

## 📌 Overview
This project implements a deep learning model for **time series prediction of PM2.5 air pollution concentration** in Ho Chi Minh City, Vietnam.  
The approach integrates **Convolutional Neural Networks (CNN)** for feature extraction and **Bidirectional Long Short-Term Memory (Bi-LSTM)** networks for temporal sequence modeling.

Air pollution, especially PM2.5, is a critical environmental issue in urban areas. Accurate forecasting helps provide early warnings, support decision-making, and protect public health.

---

## 🗂 Dataset
- **Source**: Open Development Mekong – Vietnam Air Quality Data Series (2020–2021)  
- **Location**: Ho Chi Minh City  
- **Variables used**:  
  - Temperature  
  - Humidity  
  - Wind Speed  
  - Dew Point  
  - Pressure  
  - PM2.5 concentration (target variable)  
- **Frequency**: Daily aggregated data  

---

## ⚙️ Methodology
1. **Preprocessing**
   - Data cleaning, handling missing values, and outlier treatment  
   - Feature scaling using Min-Max normalization  
   - Transforming time series into supervised learning format  

2. **Model Architecture (CNN-BiLSTM)**
   - **CNN module**: 1D Convolutions + MaxPooling for feature extraction  
   - **Bi-LSTM module**: Captures sequential dependencies in both forward and backward directions  
   - **Dense layer**: Outputs PM2.5 prediction  

3. **Baselines for comparison**
   - LSTM  
   - Bi-LSTM  
   - CNN  
   - CNN-LSTM  
   - ARIMA  

---

## 📊 Results
- Evaluation metrics: **MSE, RMSE, MAE, MAPE**  
- CNN-BiLSTM consistently outperformed baseline models, achieving **lower error rates and better prediction accuracy** on the Air Quality HCMC dataset.  
- Visualizations include training/testing loss curves and comparison plots of actual vs. predicted PM2.5 levels.

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/Truong-Thai-Bao/Air-pollution-prediction-hcmc-cnn-bilstm.git
   cd Air-pollution-prediction-hcmc-cnn-bilstm
   ```
2. Install dependencies:
  ```bash
    pip install -r requirements.txt
  ```

3. Run the Jupyter notebook:

jupyter notebook cnn_bilstm_2020.ipynb

## 📌 Requirements

- Python 3.8+

- TensorFlow / Keras

- NumPy, Pandas, Matplotlib, Seaborn

- scikit-learn

## 📖 Reference

This work is inspired by the paper:

Minh Thanh Vo, Anh H. Vo, Huong Bui, Tuong Le.
A Hybrid Deep Learning Approach for PM2.5 Concentration Prediction in Smart Environmental Monitoring.
Intelligent Automation & Soft Computing, 202x. DOI:10.32604/iasc.202x.xxxxxx

