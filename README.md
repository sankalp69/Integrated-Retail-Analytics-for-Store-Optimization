# 🛒 Integrated Retail Analytics Project

## 📌 Project Overview

This project implements an **end-to-end retail analytics pipeline** using real-world retail data to derive actionable business insights. The solution combines **data preprocessing, anomaly detection, segmentation, market basket analysis, and demand forecasting** to support better **sales optimization, inventory planning, and promotion strategies**.

The notebook demonstrates how advanced analytics and machine learning can be applied to retail data to understand customer/store behavior, detect unusual sales patterns, forecast demand, and translate insights into real-world business actions.

---

## 🎯 Business Objectives

* Detect and handle **sales anomalies** to improve data quality
* Segment **stores and departments** based on sales behavior
* Identify **product associations** to increase basket size
* Forecast **weekly sales demand** using statistical and ML models
* Use insights to design **personalized marketing and inventory strategies**

---

## 📂 Dataset Description

The project uses three primary datasets:

### 1. Sales Dataset

* **Store** – Store ID
* **Dept** – Department ID
* **Date** – Week date
* **Weekly_Sales** – Weekly sales amount

### 2. Features Dataset

* **Temperature** – Local temperature
* **Fuel_Price** – Fuel price in the region
* **CPI** – Consumer Price Index
* **Unemployment** – Unemployment rate
* **MarkDown1–5** – Promotional markdown values
* **IsHoliday** – Holiday indicator

### 3. Stores Dataset

* **Store** – Store ID
* **Type** – Store type (A, B, C)
* **Size** – Store size

---

## 🧠 Methodology & Workflow

### 1️⃣ Data Ingestion & Preprocessing

* Load and merge sales, features, and store datasets
* Handle missing values (especially markdown fields)
* Convert dates and align data at a weekly level
* Normalize and transform skewed sales data (square-root transform)

### 2️⃣ Exploratory Data Analysis (EDA)

* Sales distribution analysis
* Trend and seasonality visualization
* Identification of skewness and volatility

### 3️⃣ Anomaly Detection

* **Rolling Mean & Standard Deviation** – Detect sudden spikes/drops
* **EWMA (Exponentially Weighted Moving Average)** – Detect sustained shifts
* **Isolation Forest** – ML-based multivariate anomaly detection

📌 *Benefit:* Improves data reliability and prevents distorted forecasts

### 4️⃣ Segmentation (PCA + K-Means)

* **PCA** for dimensionality reduction
* **K-Means clustering** for store and department segmentation
* **Silhouette Score** for cluster validation

📌 *Benefit:* Enables targeted promotions and localized inventory planning

### 5️⃣ Department-wise Clustering

* Independent clustering at department level
* Identifies category-specific sales patterns

---

## 🛍️ Market Basket Analysis

* Convert transactional data into basket format
* Apply **Apriori Algorithm** to identify frequent itemsets
* Generate **association rules** using support, confidence, and lift

📌 *Benefit:* Enables cross-selling, bundling strategies, and optimized shelf placement

---

## 📈 Demand Forecasting

### 🔹 Holt-Winters Exponential Smoothing

* Captures **trend and seasonality** (weekly & yearly)
* Serves as a strong statistical baseline

### 🔹 Random Forest Regressor

* Incorporates **exogenous variables** (markdowns, holidays, economic indicators)
* Captures nonlinear relationships

📌 *Benefit:* Accurate demand forecasts for inventory replenishment and staffing decisions

---

## 🔍 Model Evaluation

* **MAE (Mean Absolute Error)**
* **RMSE (Root Mean Squared Error)**
* Forecast vs actual sales visualization

---

## 📊 Key Insights

* Markdown promotions significantly influence sales volume
* Holidays cause predictable seasonal spikes
* Stores and departments exhibit distinct sales behaviors
* ML-based forecasts outperform traditional methods when external factors are included

---

## 🚀 Business Applications

* **Personalized marketing** based on store/department segments
* **Optimized inventory levels** using demand forecasts
* **Improved cross-selling** through market basket rules
* **Reduced stockouts and overstocking**

---

## 🛠️ Technologies Used

* **Python**
* **Pandas, NumPy** – Data processing
* **Matplotlib, Seaborn** – Visualization
* **Scikit-learn** – PCA, K-Means, Isolation Forest, Random Forest
* **Statsmodels** – Holt-Winters forecasting
* **Mlxtend / Apyori** – Market Basket Analysis

---

## 📁 Project Structure

```
├── Retail_Analytics.ipynb
├── data/
│   ├── sales_data.csv
│   ├── features_data.csv
│   └── stores_data.csv
├── README.md
```

---

## 🔮 Future Enhancements

* Hierarchical forecasting (Store → Department → SKU)
* Advanced models (XGBoost, LightGBM)
* Promotion uplift & A/B testing
* Real-time anomaly monitoring dashboard

---

## 🙌 Conclusion

This project demonstrates how **data science and machine learning** can be effectively applied to retail analytics to drive **data-informed business decisions**. The modular pipeline makes it extensible and suitable for real-world deployment.

---

## 📬 Contact

For questions or collaboration:

* **Author:** [Dheeraj Patel]
* **Email:** [[patel.dheeraj98@gmail.com](mailto:patel.dheeraj98@gmail.com)]
* **LinkedIn/GitHub:** [www.linkedin.com/in/patel-dheeraj]
