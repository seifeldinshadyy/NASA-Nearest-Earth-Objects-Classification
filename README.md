# NASA-Nearest-Earth-Objects-Classification
Project Overview

This project aims to classify whether a Near-Earth Object (NEO) is hazardous or not using machine learning techniques. The dataset, sourced from NASA, contains detailed information about asteroids from 1910 to 2024.

Objectives

Data Cleaning & Preprocessing: Handle missing values efficiently and standardize numerical features.

Exploratory Data Analysis (EDA): Visualize key trends, distributions, and correlations.

Feature Engineering: Select and transform relevant features to improve model performance.

Imbalanced Data Handling: Use SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset.

Model Training & Evaluation: Train a Random Forest Classifier and evaluate it using precision, recall, F1-score, and AUC-ROC.

Dataset Details

Source: NASA Nearest Earth Objects (1910-2024) dataset

Target Variable: is_hazardous (1 = Hazardous, 0 = Non-Hazardous)

Key Features:

absolute_magnitude

estimated_diameter_min, estimated_diameter_max

relative_velocity

miss_distance

orbital_period

Methodology

Data Import & Cleaning

Loaded dataset and handled missing values.

Scaled numerical features using StandardScaler.

Exploratory Data Analysis (EDA)

Count plots for class distribution.

Correlation heatmaps and histograms for feature insights.

Data Preprocessing & Feature Selection

Removed irrelevant columns (id, name).

Applied feature scaling.

Handling Class Imbalance

Used SMOTE to generate synthetic samples for the minority class.

Model Training & Evaluation

Algorithm: Random Forest Classifier

Metrics Used: Precision, Recall, F1-Score, AUC-ROC

Result Summary: The model performed well in detecting hazardous NEOs.

Model Deployment

Saved trained model using joblib for future predictions.

Results & Key Findings

The dataset was highly imbalanced, requiring SMOTE for better model training.

Feature importance analysis showed that miss_distance and relative_velocity significantly impact classification.

The Random Forest model achieved a strong AUC-ROC score, making it reliable for identifying hazardous objects.
