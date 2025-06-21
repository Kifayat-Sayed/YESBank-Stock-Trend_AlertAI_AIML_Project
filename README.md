# 🏦 YES Bank Stock Trend & Price Prediction

Dual-Model ML System for Stock Trend Classification and Closing Price Forecasting

A comprehensive machine learning project designed to assist investors and analysts in understanding and predicting the short-term behavior of YES Bank stock. This project combines classification and regression models to provide robust insights and predictions.

---

## 🌟 Key Features

### ✅ Stock Trend Classification

Predicts whether the stock price will **Rise (1)** or **Fall (-1)** using engineered features such as:

* Price Range
* Volatility (%)
* Monthly Return (%)
* Historical OHLC values

🔍 Classification Models Used:

* Logistic Regression
* Random Forest Classifier
* XGBoost Classifier

> 📈 **Best Model**: XGBoost
> 📊 **Accuracy**: 100% on test set *(due to dataset characteristics, small size)*

---

### ✅ Next-Day Closing Price Prediction

Forecasts the **next day's closing stock price** using past trends and technical indicators like:

* Moving Averages (MA\_3, MA\_6)
* Volatility
* Open, High, Low, Close values

🔍 Regression Models Used:

* Ridge Regression
* Random Forest Regressor
* Gradient Boosting Regressor
* XGBoost Regressor

> 📈 **Best Model**: Gradient Boosting Regressor
> 📊 **R² Score**: 0.6087 (Test Set)
> 📊 **CV R²**: 0.7620 ± 0.1542

---

## 🔍 Project Overview

### 1. Stock Trend Classifier

**Objective**: Classify monthly stock movement into `Rise` or `Fall`.
**Approach**: Engineered labels based on closing vs. opening price.
**Output**: Binary classification (1 for Rise, -1 for Fall)
**Best Model**: XGBoost

---

### 2. Closing Price Predictor

**Objective**: Predict the next month's closing price.
**Approach**: Supervised regression using technical indicators.
**Output**: Continuous closing price prediction
**Best Model**: Gradient Boosting Regressor

---

## 🧪 ML Models Used

* 🔹 Logistic Regression
* 🔹 Ridge, Lasso, ElasticNet
* 🔹 Random Forest
* 🔹 Gradient Boosting
* 🔹 XGBoost (Classifier + Regressor)

All models include:

* Hyperparameter tuning (GridSearchCV, RandomizedSearchCV)
* Cross-validation using TimeSeriesSplit

---

## 📈 Evaluation Metrics

**Classification Models**:

* Accuracy, Precision, Recall, F1 Score
* Confusion Matrix
* Macro-averaged metrics for class balance

**Regression Models**:

* RMSE (Root Mean Squared Error)
* MAE (Mean Absolute Error)
* R² Score
* Cross-validation R²

---

## 📊 Data Visualization & Analysis

Structured using the **UBM Framework**:

* 🔹 **Univariate Analysis**: Distribution, volatility, return histograms
* 🔹 **Bivariate Analysis**: Open vs Close, High vs Low, Volatility vs Return
* 🔹 **Multivariate Analysis**: Pairplots, Correlation Heatmaps

> ✅ Over 15 charts with clear business justifications and actionable insights

---

## 🧠 Feature Engineering & Preprocessing

* Rolling Moving Averages (MA\_3, MA\_6)
* Volatility (%)
* Monthly Return (%)
* Price Movement Labeling
* IQR-based outlier treatment
* StandardScaler & RobustScaler

---

## 🔬 Hypothesis Testing Conducted

* 🔹 Is the average monthly return different from zero? *(T-test)*
* 🔹 Are returns significantly different for gain vs loss months? *(Welch's T-test)*
* 🔹 Is volatility higher in negative return years? *(One-tailed test)*

---

## 💾 Saved Models

Models saved using `joblib` for deployment.
✅ Example:

```python
joblib.dump(gb_best, 'gradient_boosting_model.pkl')
```

---

## 🚀 Deployment Ready

This project is **production-ready** and can be deployed using:

* **Streamlit** dashboard for real-time stock prediction
* **Flask or FastAPI** for backend APIs
* Integrated into financial dashboards or trading tools

---

## 🧠 What I Learned

* Built a dual-model ML system combining classification and regression
* Applied advanced feature engineering using financial domain logic
* Performed robust cross-validation with time-series splits
* Learned about SHAP/LIME (model explainability), although not included
* Improved understanding of financial modeling and forecasting with ML

---

## 💡 How This Helps Me

Enhances my ability to:

* Solve real-world financial prediction problems
* Apply machine learning to time-series data
* Interpret ML models and communicate business value
* Strengthen my profile for roles in FinTech, AI/ML, and Data Science

---

## ✍️ Author

**Kifayat Sayed**
M.Sc. AI & ML | Data Science
📧 [kifayatsayed301@gmail.com](mailto:kifayatsayed301@gmail.com)
🌐 [LinkedIn](https://linkedin.com/in/kifayat-sayed) | [GitHub Portfolio](https://github.com/Kifayat-Sayed)

