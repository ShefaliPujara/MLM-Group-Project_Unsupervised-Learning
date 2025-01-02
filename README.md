# MLM-Group-Project_Unsupervised-Learning
1. Project Information


Project Title : Application of Machine Learning for Imports-Exports Dataset Analysis

Made by : 055044, Shefali Pujara 

Group No : Group 8

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



3. Project Objectives & Problem Statements
Unsupervised Machine Learning: Clustering

Project Objectives:

Segmentation of the imports-exports dataset using unsupervised machine learning clustering algorithms (K-Means).

Identification of the optimal number of clusters for the dataset based on evaluation metrics (Silhouette Score, Davies-Bouldin Score).

Characterization of the identified clusters based on the distribution of variables like Quantity, Value, Weight, Import_Export, Category, Shipping_Method, and Payment_Terms.


Problem Statements:

How can the imports-exports dataset be effectively segmented into meaningful clusters using K-Means clustering?

What is the most appropriate number of clusters for representing the underlying structure of the data?

What are the key characteristics and distinguishing features of each identified cluster in terms of the included variables?


Overall Observations and Findings

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


6. Managerial Insights and Recommendations
Insights:


Data-Driven Segmentation: Cluster analysis revealed distinct customer segments based on transaction characteristics (Quantity, Value, Weight). This segmentation can inform targeted marketing, inventory management, and logistics strategies.

Predictive Model Limitations: Machine learning models using only Quantity and Weight as features demonstrated limited accuracy in predicting Import/Export status. This highlights the need for richer data and potentially more sophisticated models for reliable predictions.

Model Comparison: While Decision Tree showed marginally better accuracy in this specific case, Random Forest and XGBoost offer advantages like robustness to overfitting and potential for better generalization. Choosing the right model requires considering performance, interpretability, and computational efficiency.

Feature Importance: Understanding the relative importance of different features for prediction is crucial for effective decision-making. Further analysis is needed to identify key drivers of Import/Export status.


Recommendations:

Leverage Customer Segmentation: Tailor business strategies to the identified customer segments, such as offering customized pricing, promotions, or logistics solutions based on their typical transaction characteristics.

Enhance Data Collection: Explore opportunities to collect more comprehensive data, including product category, shipping method, payment terms, and other relevant variables, to improve predictive model accuracy.

Feature Engineering: Explore feature interactions and create new derived features that might capture more complex relationships between variables and enhance model performance.

Model Refinement: Further evaluate model performance using hyperparameter tuning, cross-validation, and alternative algorithms to identify the most accurate and robust model for predicting Import/Export status.

Operational Optimization: Use model insights to optimize operational processes, such as inventory management (based on typical order quantities and product value), warehouse layout (based on product weight and size), and logistics planning (based on shipping methods and destination countries).

Continuous Monitoring: Establish a system for ongoing monitoring of model performance and data patterns to adapt strategies as needed and ensure continued effectiveness.

Data-Driven Decision Making: Encourage a data-driven culture within the organization, leveraging insights from the analysis to inform strategic decisions and improve overall business outcomes.
