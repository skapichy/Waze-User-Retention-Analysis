# Waze-User-Retention-Analysis
This project investigates user retention patterns within the Waze navigation app using a real-world dataset of 14,999 users. By applying machine learning techniques, the aim was to predict whether a user will be retained or churned based on behavioral metrics such as session frequency, navigation habits, and driving activity. The analysis includes data cleaning, feature engineering, model building, and performance evaluation using logistic regression.


# Project Summary
- Dataset: 14,999 rows, 13 features including user activity, navigation behavior, and retention labels.
- Target Variable: label (retained vs. churned)
- Model Used: Logistic Regression
- Evaluation Metrics: Accuracy, Precision, Recall, F1 Score, Confusion Matrix
- Outcome: Achieved a recall of 100%, indicating strong sensitivity to identifying retained users, though precision and accuracy suggest room for model refinement.


# Tools and Technologies
- Python
- pandas, NumPy - Data Manipulation
- seaborn, matplotlib - Data Visualization
- scikit-learn - Machine Learning (LogisticRegression, train_test_split, metrics)
- OneHotEncoder, StandardScaler - For Preprocessing
- Jupyter Notebook - project Environment


# Project Objectives
- Clean and preprocess raw user activity data
- Engineer relevant features for predictive modeling
- Build a classification model to predict user retention
- Evaluate model performance using standard metrics
- Visualize trends and patterns in user behavior
- Generate actionable insights for product and marketing teams


# Data Pipeline Overview
- Data Loading: Imported CSV file using pandas
- Exploratory Data Analysis (EDA): Summary statistics, missing value handling, value counts
- Data Cleaning: Dropped irrelevant columns (e.g., ID), removed nulls
- Feature Engineering: One-hot encoding for categorical variables (label, device)
- Modeling: Logistic regression using scikit-learn
- Evaluation: Confusion matrix, accuracy, precision, recall, F1 score
- Visualization: Regression plots, heatmaps, bar charts


# Business Insights
- Retention Dominance: Majority of users are retained, indicating strong engagement.
- Activity Correlation: Higher session counts and navigation frequency correlate with retention.
- Model Behavior: The classifier predicts all users as retained, leading to high recall but low precision—suggesting class imbalance or feature limitations.
- Feature Importance: Variables like driven_km_drives, duration_minutes_drives, and total_navigations_fav1 show strong influence on retention.


# Recommendations
- Model Refinement: Address class imbalance using techniques like SMOTE or ensemble methods.
- Feature Expansion: Incorporate time-based features (e.g., recency, frequency) and user segmentation.
- Business Strategy:
- Target users with declining navigation activity for re-engagement campaigns.
- Use predictive insights to personalize onboarding and retention strategies.
- Product Development: Enhance features that drive engagement such as favorite navigation routes and session frequencies.


