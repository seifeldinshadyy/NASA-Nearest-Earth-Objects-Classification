# NASA-Nearest-Earth-Objects-Classification
Project Overview:
This project aims to classify whether a Near-Earth Object (NEO) is hazardous or not using machine learning techniques. The dataset, sourced from NASA, contains detailed information about asteroids from 1910 to 2024.

Objectives

1.Data Cleaning & Preprocessing: Handle missing values efficiently and standardize numerical features.
2.Exploratory Data Analysis (EDA): Visualize key trends, distributions, and correlations.
3.Feature Engineering: Select and transform relevant features to improve model performance.
4.Imbalanced Data Handling: Use SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset.
5.Model Training & Evaluation: Train a Random Forest Classifier and evaluate it using precision, recall, F1-score, and AUC-ROC.

Dataset Details

Source: NASA Nearest Earth Objects (1910-2024) dataset
Target Variable: is_hazardous (1 = Hazardous, 0 = Non-Hazardous)
Key Features:
1.absolute_magnitude
2.estimated_diameter_min, estimated_diameter_max
3.relative_velocity
4.miss_distance
5.orbital_period

Methodology
1.Data Import & Cleaning
   1.1Loaded dataset and handled missing values.
   1.2Scaled numerical features using StandardScaler.
2.Exploratory Data Analysis (EDA)
   2.1Count plots for class distribution.
   2.2Correlation heatmaps and histograms for feature insights.
3.Data Preprocessing & Feature Selection
    3.1Removed irrelevant columns (id, name).
    3.2Applied feature scaling.
4.Handling Class Imbalance
  4.1Used SMOTE to generate synthetic samples for the minority class.
5.Model Training & Evaluation
   5.1Algorithm: Random Forest Classifier
   5.2Metrics Used: Precision, Recall, F1-Score, AUC-ROC
   5.3Result Summary: The model performed well in detecting hazardous NEOs.
6.Model Deployment
  6.1Saved trained model using joblib for future predictions.


Results & Key Findings
The dataset was highly imbalanced, requiring SMOTE for better model training.
Featureimportance analysis showed that miss_distance and relative_velocity significantly impact classification.
The Random Forest model achieved a strong AUC-ROC score, making it reliable for identifying hazardous objects.
