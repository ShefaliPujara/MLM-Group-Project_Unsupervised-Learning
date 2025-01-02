# MLM-Group-Project_Unsupervised-Learning


## Project Information

### Project Title
- **Application of Machine Learning for Imports-Exports Dataset Analysis**

### Made by
- **055044, Shefali Pujara**

---

## Description of Data

- **Data Source:** Kaggle Imports-Exports Dataset  
- **Data Size:** ~2 MB  
- **Data Type:** Cross-sectional  
- **Data Dimension:** 16 Variables, 15,000 Observations  

### Data Variable Type
- **Numeric:** Integer, Decimal  
- **Non-Numeric:** Categorical  

### Data Variable Categories
1. **Category-I**  
   - **Index:** Transaction_ID  
   - **Categorical (Nominal):** Country, Product, Import_Export, Shipping_Method  
   - **Categorical (Ordinal):** Payment_Terms  
   - **Non-Categorical:** Quantity, Value, Weight  
2. **Category-II**  
   - **Input Variables or Features:** All variables except Import_Export  
   - **Outcome Variable(s) or Feature(s):** Import_Export  

### About Dataset
- Contains transactional records of imports and exports across various countries, products, and ports.  
- Includes details about shipment weight, value, and shipping methods.  
- Provides scope for clustering and classification tasks.

---

## Executive Summary

- Comprehensive analysis of imports-exports dataset.  
- Objectives: Preprocess data, identify patterns, and develop predictive models.  
- Techniques: Descriptive statistics, clustering, supervised ML, and data transformation.  
- Insights: Explored relationships between variables, assessed normality, and managed outliers.

---

## Project Goals and Objectives

1. Prepare the dataset for advanced analytics and machine learning.  
2. Effectively manage and impute missing data.  
3. Transform categorical data into numerical format.  
4. Standardize and normalize numerical data, including testing for normality.  
5. Identify natural groupings within transactional data.  
6. Assess relationships between categorical variables using a test of homogeneity.  
7. Develop predictive models for shipping methods.  
8. Evaluate and compare machine learning model performance.  
9. Generate actionable business insights.

---

## Methodology

1. **Data Acquisition and Preparation**  
   - Data cleaning, missing data imputation, encoding, and scaling.  
   - Managed outliers through row and column removal.  

2. **Exploratory Data Analysis (EDA)**  
   - Descriptive statistics and visualizations.  
   - Central tendency, dispersion, variable relationships.  

3. **Normality Testing**  
   - Applied Shapiro-Wilk, Kolmogorov-Smirnov, Anderson-Darling, and Jarque-Bera tests.  

4. **Test of Homogeneity**  
   - Chi-squared test to evaluate independence of categorical variables.  

5. **Cluster Analysis**  
   - K-Means clustering using Quantity, Value, and Weight.  
   - Evaluated using silhouette and Davies-Bouldin scores.  

6. **Supervised Learning**  
   - Models: Decision Tree, Logistic Regression, Random Forest, XGBoost.  
   - Predictors: Quantity and Weight.  

7. **Model Evaluation and Comparison**  
   - Metrics: Accuracy, classification reports, confusion matrices.  

8. **Insight Generation**  
   - Business recommendations derived from EDA and model results.

---

## Overall Observations and Findings

- **Data Quality:** Relatively clean dataset.  
- **Data Scaling:** Improved model performance with scaled non-categorical features.  
- **Clustering Insights:** Identified distinct data segments.  
- **Model Performance:**  
  - Logistic Regression: ~0.35 accuracy.  
  - Decision Tree: ~0.32 accuracy.  
  - Random Forest: ~0.32 accuracy.  
  - XGBoost: ~0.31 accuracy.  
- **Feature Importance:** Requires further analysis.  
- **Model Selection:** Decision Tree preferred; Random Forest and XGBoost also viable.  
- **Further Improvements:** Feature engineering, hyperparameter tuning, alternative algorithms.

---

## Managerial Insights and Recommendations

### Insights
1. **Data-Driven Segmentation**  
   - Cluster analysis revealed distinct customer segments based on transaction characteristics.  

2. **Predictive Model Limitations**  
   - Limited accuracy with current features; richer data needed.  

3. **Model Comparison**  
   - Decision Tree marginally better; Random Forest and XGBoost offer robustness.  

4. **Feature Importance**  
   - Further analysis required to identify key drivers of Import/Export status.  

### Recommendations
1. Tailor strategies for identified customer segments (e.g., pricing, promotions, logistics).  
2. Enhance data collection (e.g., product category, shipping method, payment terms).  
3. Explore feature engineering for complex relationships.  
4. Refine models with hyperparameter tuning and cross-validation.  
5. Optimize operations based on model insights (e.g., inventory management, logistics planning).  
6. Continuously monitor model performance and adapt strategies.  
7. Foster a data-driven culture for strategic decision-making.


