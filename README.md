# 🌫️ PM2.5 Air Pollution Prediction with CNN–BiLSTM

## 📌 Introduction
This project focuses on predicting fine particulate matter (PM2.5) concentrations in Ho Chi Minh City using a **hybrid deep learning model**. The approach combines **Convolutional Neural Networks (CNN)** for feature extraction and **Bidirectional Long Short-Term Memory (Bi-LSTM)** for capturing temporal dependencies.  

The project improves upon the baseline PM25-CBL model by optimizing parameters, reducing complexity, and achieving higher prediction accuracy.

---

## 📊 Dataset
- **Source:** Air Quality HCMC dataset (Open Development Mekong, 2020)  
- **Features used:**  
  - Temperature  
  - Humidity  
  - Wind Speed  
  - Dew  
  - Pressure  
  - PM2.5 (target variable)  
- **Preprocessing:** Missing value handling, normalization using Min–Max scaling, train/test split (80/20).  

---

## 🏗️ Methodology
1. **Data Preprocessing**
   - Handle missing values
   - Normalize features with Min–Max Scaler
   - Create time-series sequences  

2. **Model Architecture**
   - **CNN (Separable Convolution):** Extract local temporal features  
   - **Bi-LSTM:** Learn bidirectional time dependencies  
   - **Fully Connected Layer:** Output PM2.5 prediction  

3. **Evaluation Metrics**
   - MSE (Mean Squared Error)  
   - RMSE (Root Mean Squared Error)  
   - MAE (Mean Absolute Error)  
   - MAPE (Mean Absolute Percentage Error)  

---

## 🚀 Results
- The proposed **PM25-CBLo model** significantly outperformed baseline models (CNN, LSTM, Bi-LSTM, CNN-LSTM, PM25-CBL).  
- **Best performance:**  
  - MSE: 0.907  
  - RMSE: 0.952  
  - MAE: 0.762  
  - MAPE: 2.909%  

The optimized CNN–BiLSTM architecture reduced parameters by ~3x compared to PM25-CBL, while improving accuracy and lowering computational cost.

---


---

## ⚙️ Technologies
- Python 3.x  
- Google Colab  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- Scikit-learn  
- TensorFlow/Keras  

---

## 📈 Future Work
- Extend to multi-step forecasting (predicting multiple future time steps).  
- Integrate external features (e.g., traffic, satellite data).  
- Deploy as a real-time monitoring dashboard.  

---

## 📚 References
- Vo, M.T. et al. (2023). *A Hybrid Deep Learning Approach for PM2.5 Concentration Prediction in Smart Environmental Monitoring.* Intelligent Automation & Soft Computing, 36(3), 3029–3041.  
- Open Development Mekong (2020). *Dataset on Air Quality in Vietnam.*  

