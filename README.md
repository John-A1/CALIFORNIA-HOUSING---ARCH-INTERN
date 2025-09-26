# CALIFORNIA-HOUSING---ARCH-INTERN

# 🏡 California Housing Price Prediction with Neural Networks  

This project demonstrates how to build a **Neural Network Regressor** using **TensorFlow/Keras** to predict **median house values** in California.  
We use the **California Housing dataset** from `scikit-learn`, apply preprocessing (scaling, outlier handling), and evaluate the model with **R² Score**.  

---

## 📌 Objective  
- Train a neural network to predict **California median house prices**.  
- Apply **data preprocessing** (handling missing values, duplicates, outliers, scaling).  
- Evaluate regression performance using **Mean Squared Error (MSE)** and **R² Score**.  

---

## 📊 Dataset  
The [California Housing dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html) is a classic dataset derived from the **1990 U.S. Census**.  

- **Features (8):**  
  - MedInc – Median income in block group  
  - HouseAge – Median house age in block group  
  - AveRooms – Average number of rooms per household  
  - AveBedrms – Average number of bedrooms per household  
  - Population – Block group population  
  - AveOccup – Average household size  
  - Latitude – Block group latitude  
  - Longitude – Block group longitude  

- **Target:**  
  - `MedHouseVal` → Median house value (in 100,000 USD)  

---

## ⚙️ Project Workflow  

### **1. Data Loading & Saving**  
- Load California housing dataset via `fetch_california_housing`.  
- Save dataset as CSV for reuse.  

### **2. Data Cleaning & Preprocessing**  
- Handle **missing values** & **duplicates**.  
- Handle outliers using **Z-Score** filtering.  
- Feature scaling with **StandardScaler**.  
- Train-test split (80/20).  

### **3. Neural Network Model**  
A simple **feedforward neural network**:  
- Optimizer: **Adam**  
- Loss: **Mean Squared Error (MSE)**  

### **4. Training**  
- Epochs: **50**  
- Batch size: **8**  
- Validation data: 20% split  

### **5. Evaluation**  
- Metric: **R² Score**  
- Achieved **R² = 0.7954 (~79.5%)**, meaning the model explains ~79% of the variance in housing prices.  

---

## 📈 Results  

✅ Model learns effectively with decreasing loss.  
✅ R² score close to **0.80** → good predictive performance for a baseline neural network.  
⚠️ Further tuning (more layers, dropout, regularization) can improve results. 
