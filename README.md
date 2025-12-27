# Divar Real Estate Analysis & Prediction

## Project Overview
This project performs a comprehensive analysis of the Iranian real estate market using a dataset of **over 1 million ads** from the **Divar** platform. The goal was to transform raw, unstructured data into actionable insights and accurate price prediction models.

Our team engineered a complete data pipeline that includes data cleaning, exploratory data analysis (EDA), geospatial clustering, and machine learning regression models.

## Mentor 
**Aryan**

## Team Members 
**Sasan,** 
**Mohammad,**
**Amin,**
**Mahyar**

---

## Key Features & Modules

### 1. Robust Data Pipeline & Cleaning
> *Foundations of the analysis.*
* **Data Cleaning:** Handled missing values (imputation strategies for `construction_year` and amenities), standardized Persian dates/numbers, and fixed inconsistent data types.
* **Outlier Detection:** Applied statistical methods to remove anomalies in pricing and square footage to ensure model stability.
* **Feature Engineering:** Created high-value features such as `luxury_score` (based on pools/saunas), `building_age`, and location-based flags.

### 2. Exploratory Data Analysis (EDA)
> *Visualizing market dynamics.*
* **Market Trends:** Analyzed percentage price changes over time to identify inflation impacts and seasonal demand spikes.
* **Distribution Analysis:** visualized the spread of property types, construction years, and ad categories (Rent vs. Sell).
* **Geospatial Mapping:** Created heatmaps to identify high-density zones and luxury neighborhoods across major cities.

### 3. Advanced Clustering (Unsupervised Learning)
> *Segmenting the market.*
* **K-Means Clustering:** Grouped neighborhoods into distinct segments based on price per meter and location.
* **DBSCAN:** Implemented density-based clustering to identify core housing clusters and separate them from noise/outliers.

### 4. Price Prediction (Supervised Learning)
> *Forecasting property values.*
* **Regression Modeling:** Developed Machine Learning models to predict property prices based on features like area, location, and amenities.
* **Evaluation:** Optimized models to minimize error rates (RMSE/MAE), providing reliable price estimates for users.

---

## 📂 Repository Structure

The project is organized into logical modules covering the entire workflow:

```text
├── data/                       # Raw and processed datasets
├── notebooks/
│   ├── 01_Data_Cleaning.ipynb  # Primary cleaning pipeline & preprocessing
│   ├── 02_EDA_Charts.ipynb     # General market visualization & distributions
│   ├── FeatureEngineering.ipynb# Creation of derived features (Luxury Score, etc.)
│   ├── clustering_divar.ipynb  # K-Means implementation
│   ├── DBScan_Clustering.ipynb # Density-based clustering (DBSCAN)
│   ├── prediction.ipynb        # Price prediction models (Regression)
│   └── percentage_price_change.ipynb # Time-series analysis of prices
├── Images/                     # Exported plots and heatmap results
└── README.md                   # Project documentation
