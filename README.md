# MLM-Group-Project_Unsupervised-Learning
1. Project Information


Project Title : Application of Machine Learning for Imports-Exports Dataset Analysis

Made by : 055044, Shefali Pujara 



2. Description of Data


Data Source: Kaggle Imports-Exports Dataset


Data Size: ~2 MB


Data Type: Cross-sectional


Data Dimension: 16 Variables, 15,000 Observations


Data Variable Type:


Numeric: Integer, Decimal


Non-Numeric: Categorical


Data Variable Category-I:


Index: Transaction_ID


Categorical (Nominal): Country, Product, Import_Export, Shipping_Method


Categorical (Ordinal): Payment_Terms


Non-Categorical: Quantity, Value, Weight


Data Variable Category-II:


Input Variables or Features: All variables except Import_Export


Outcome Variable(s) or Feature(s): Import_Export


About Dataset: The dataset contains transactional records of imports and exports across various countries, products, and ports. It includes details about shipment weight, value, and shipping methods, providing ample scope for clustering and classification tasks.



3. Executive Summary

This report summarizes the findings of a comprehensive data analysis project focused on an imports-exports dataset. The project's core objectives were to preprocess and explore the data, identify inherent patterns and groupings, and develop predictive models to understand key aspects of the import-export process. Through a systematic approach encompassing descriptive statistics, data transformation, clustering, and supervised machine learning techniques, the project successfully uncovered actionable insights and built models that provide predictive capabilities for critical business decisions. Notably, the project also delved into the relationships between categorical variables, assessed the normality of numerical variables, and carefully handled data outliers, adding depth to the overall analysis.

4. Project Goals and Objectives

The project was initiated to address the following key objectives:

Prepare the dataset for advanced analytics and machine learning.
Effectively manage and impute missing data.
Transform categorical data into a usable numerical format.
Standardize and normalize numerical data, including rigorous testing for normality.
Identify natural groupings within the transactional data.
Assess the relationships between categorical variables using a test of homogeneity.
Develop predictive models to understand and forecast shipping methods.
Evaluate and compare the performance of different machine learning models.
Generate business insights from the analysis, applicable to strategy and operations.

 5. Methodology

The project followed a multi-phased methodology:

Data Acquisition and Preparation: The dataset was acquired, loaded, and subjected to rigorous data cleaning and preprocessing, including missing data handling (imputation), categorical data encoding (Ordinal Encoding), and numerical data scaling (MinMaxScaler). Outliers were considered during this stage and managed via row and column removal.
Exploratory Data Analysis (EDA): Descriptive statistics and visualizations were utilized to understand data characteristics, including central tendency, dispersion, variable relationships, and categorical distributions.
Normality Testing: Rigorous testing was applied to the numerical variables. Tests applied were shapiro-Wilk, Kolmogorov-Smirnov, Anderson-Darling, and Jarque-Bera tests.
Test of Homogeneity: A chi-squared test of homogeneity was implemented to test the independence of all categorical variables.
Cluster Analysis: K-Means clustering was employed to segment transactional data based on key numerical variables (Quantity, Value, Weight). The optimal number of clusters was evaluated using silhouette and Davies-Bouldin scores.
Supervised Learning: Supervised machine learning models, including Decision Tree, Logistic Regression, Random Forest and XGBoost, were trained to predict the 'Shipping_Method' using 'Quantity' and 'Weight' as predictors.
Model Evaluation and Comparison: The models were rigorously evaluated using relevant metrics such as accuracy, classification reports, and confusion matrices. A comparative analysis of model performance was conducted.
Insight Generation: Insights derived from EDA, cluster analysis, and model results were translated into actionable business recommendations.


6. Overall Observations and Findings

Data Quality: The dataset was relatively clean, facilitating analysis.

Data Scaling: Non-categorical features were scaled for model improvement.

Clustering Insights: K-Means identified distinct data segments.

Logistic Regression: Low accuracy (~0.35) for Import/Export prediction.

Decision Tree: Slightly better accuracy (~0.32) than Logistic Regression and Random Forest in this case.

Random Forest: Similar accuracy (~0.32) to Logistic Regression, less prone to overfitting than Decision Tree.

XGBoost: Comparable accuracy (~0.31) to Random Forest and Logistic Regression, potentially more efficient.

Feature Importance: Further analysis needed to identify important features.

Model Selection: Decision Tree might be preferred, but consider Random Forest and XGBoost.

Further Improvements: Explore feature engineering, hyperparameter tuning, and alternative algorithms. """


7. Managerial Insights and Recommendations
Insights:


Data-Driven Segmentation: Cluster analysis revealed distinct customer segments based on transaction characteristics (Quantity, Value, Weight). This segmentation can inform targeted marketing, inventory management, and logistics strategies.

Predictive Model Limitations: Machine learning models using only Quantity and Weight as features demonstrated limited accuracy in predicting Import/Export status. This highlights the need for richer data and potentially more sophisticated models for reliable predictions.

Model Comparison: While Decision Tree showed marginally better accuracy in this specific case, Random Forest and XGBoost offer advantages like robustness to overfitting and potential for better generalization. Choosing the right model requires considering performance, interpretability, and computational efficiency.

Feature Importance: Understanding the relative importance of different features for prediction is crucial for effective decision-making. Further analysis is needed to identify key drivers of Import/Export status.


8. Recommendations:

Leverage Customer Segmentation: Tailor business strategies to the identified customer segments, such as offering customized pricing, promotions, or logistics solutions based on their typical transaction characteristics.

Enhance Data Collection: Explore opportunities to collect more comprehensive data, including product category, shipping method, payment terms, and other relevant variables, to improve predictive model accuracy.

Feature Engineering: Explore feature interactions and create new derived features that might capture more complex relationships between variables and enhance model performance.

Model Refinement: Further evaluate model performance using hyperparameter tuning, cross-validation, and alternative algorithms to identify the most accurate and robust model for predicting Import/Export status.

Operational Optimization: Use model insights to optimize operational processes, such as inventory management (based on typical order quantities and product value), warehouse layout (based on product weight and size), and logistics planning (based on shipping methods and destination countries).

Continuous Monitoring: Establish a system for ongoing monitoring of model performance and data patterns to adapt strategies as needed and ensure continued effectiveness.

Data-Driven Decision Making: Encourage a data-driven culture within the organization, leveraging insights from the analysis to inform strategic decisions and improve overall business outcomes.
