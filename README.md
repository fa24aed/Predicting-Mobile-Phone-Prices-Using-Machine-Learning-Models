---
# 📱 Mobile Phone Price Prediction

A machine learning project that predicts mobile phone prices using various regression models, including Random Forest, Gradient Boosting, and XGBoost.

---

## 🚀 Project Overview

This project builds a complete end-to-end machine learning pipeline to estimate mobile phone prices based on their specifications such as:

* RAM
* Storage
* Battery capacity
* Screen size
* Camera features
* Processor and brand

The goal is to compare multiple models and identify the best-performing one using robust evaluation metrics.

---

## 📂 Dataset

The dataset contains mobile phone specifications and corresponding prices.

**Key Features:**

* Numerical: RAM, Storage, Battery Capacity, Screen Size
* Categorical: Brand, Processor
* Binary: Wi-Fi, Bluetooth, GPS, 4G/5G support

---

## ⚙️ Workflow

### 1. Data Preprocessing

* Removed duplicates
* Handled missing values:

  * Median for numerical features
  * Mode for categorical features
* Converted binary features (Yes/No → 1/0)

---

### 2. Feature Engineering

Created meaningful features such as:

* Storage-to-RAM ratio
* Battery per screen size
* Pixels per inch (PPI)
* Total camera pixels

---

### 3. Exploratory Data Analysis (EDA)

* Correlation heatmap
* Scatter plots with regression trends
* Boxplots for:

  * Processor vs Price
  * Brand vs Price

---

### 4. Model Training

The following models were trained and compared:

* 🌲 Random Forest Regressor
* 🌿 Gradient Boosting Regressor
* 🚀 XGBoost Regressor

---

### 5. Model Evaluation

Models were evaluated using:

* **MAE (Mean Absolute Error)**
* **RMSE (Root Mean Squared Error)**
* **R² Score (Coefficient of Determination)**

Additional analysis:

* Actual vs Predicted plots
* Error distribution (E-Pop plots)

---

### 6. Hyperparameter Optimization

Performed using **RandomizedSearchCV** with cross-validation for:

* Random Forest
* Gradient Boosting
* XGBoost

---

## 📊 Results

The models were compared based on performance metrics:

| Model             | MAE            | MAE            | R²             |
| ----------------- | -------------- | -------------- | -------------- |
| Random Forest     | 3685.48        | 9420.02        | 0.663          |
| Gradient Boosting | 3746.46        | 9451.67        | 0.661          |
| XGBoost           | 3450.45        | 9297.31        | 0.672          |

> 🏆 The best model is selected based on combined performance across all metrics.

---

## 📈 Visualizations

The project includes:

* Correlation heatmap
* Feature vs price scatter plots
* Actual vs predicted comparison plots
* Error distribution histograms
* Model comparison bar charts

---

## 🛠️ Technologies Used

* Python 🐍
* Pandas & NumPy
* Matplotlib & Seaborn
* Scikit-learn
* XGBoost

3. Run the notebook or script

---

## 📌 Key Learnings

* Importance of feature engineering in regression tasks
* Comparing ensemble models for structured data
* Hyperparameter tuning using cross-validation
* Evaluating models beyond a single metric

---
