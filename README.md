# 🏠 House Price Prediction using Machine Learning

## 📌 Project Overview
This project aims to build a **robust machine learning model** to accurately predict house prices based on various structural, locational, and functional features. The goal was to analyze the dataset, perform systematic preprocessing, compare multiple models, and select the best-performing one for real-world deployment.

---

## 🎯 Objective
- To understand the key factors influencing house prices  
- To build and evaluate multiple regression models  
- To select the most accurate and reliable model for prediction  

---

## 📊 Dataset
- Contains information about residential properties including:
  - Property size, quality, garage features, air conditioning, etc.
- Target variable: **SalePrice**

---

## 🛠️ Methodology

### 🔹 1. Data Preprocessing
- Handling missing values (median for numerical, mode for categorical)
- Outlier detection and treatment using IQR
- Encoding categorical variables (Label Encoding / One-Hot Encoding)
- Feature scaling using StandardScaler

### 🔹 2. Exploratory Data Analysis (EDA)
- Univariate analysis (histograms, distributions)
- Bivariate analysis (scatter plots with SalePrice)
- Correlation heatmap and multicollinearity handling

### 🔹 3. Feature Selection
- Identified and removed highly correlated features
- Analyzed feature importance using XGBoost

### 🔹 4. Model Building
Implemented and compared the following models:
- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest Regression
- Gradient Boosting Regression
- **XGBoost Regression (Best Model)**

### 🔹 5. Model Evaluation
Models were evaluated using:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score
- Adjusted R² Score

---

## 🏆 Best Performing Model: **XGBoost Regression**
XGBoost outperformed all other models with:
- Lowest prediction error (MAE, MSE, RMSE)
- Highest R² and Adjusted R² score  
- Stable performance validated using:
  - Actual vs Predicted plot  
  - Residual analysis  

---

## 🔍 Key Findings (Business Insights)
- **Overall Quality** and **Garage Finish** were the most influential features.
- Houses with **central air conditioning** and **more garage capacity** tend to have higher prices.
- Newer houses generally have better valuation.
- Model behavior aligns well with real-world housing trends.

---

## 📂 Files in this Repository
- `HousePricePred.ipynb` → Complete analysis and model implementation  
- `data.csv` → Dataset used in this project  

---

## 🚀 Future Scope
- Hyperparameter tuning of XGBoost
- Deploy the model using **Streamlit or Flask**
- Build a web-based house price prediction app

---

## 🛠️ Tools & Libraries Used
- Python, Pandas, NumPy  
- Scikit-learn, XGBoost  
- Matplotlib, Seaborn  
