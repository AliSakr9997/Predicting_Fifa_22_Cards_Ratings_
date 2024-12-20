FIFA 22 Player Ratings Prediction
This project uses machine learning to predict FIFA 22 player ratings based on player attributes. By analyzing the dataset and applying regression models, we aim to develop an accurate predictive model and identify key features that influence player ratings.

Project Overview
The goal of this project is to predict FIFA player ratings using attributes such as "Reactions," "Composure," and "Shot Power." This is a regression problem where we evaluated various machine learning models to identify the best-performing one and optimize its performance.

Key highlights include:

Cleaning and preprocessing the data.
Evaluating multiple regression models.
Optimizing the Random Forest model using hyperparameter tuning.
Interpreting results to provide meaningful insights into player performance.
Dataset
Source: FIFA 22 player data containing 16,501 entries and 65 features.
Features Include: Player attributes like "Pace," "Shooting," "Passing," and metadata such as nationality and club.
Target Variable: Overall player rating.
Data Preprocessing
Removed irrelevant features (e.g., Player IDs, Photos, and Current Club).
Addressed missing values by dropping sparse columns (e.g., "Marking") and rows with missing data.
Final cleaned dataset size: 15,612 entries.
Split data into training (70%) and testing (30%) sets, with shuffle=True for randomness.
Models and Evaluation
Three regression models were tested:

Linear Regression
Decision Tree
Random Forest (performed best)
Evaluation Metrics
Root Mean Squared Error (RMSE): Measures error magnitude.
R² (Coefficient of Determination): Indicates how well the model explains variance.
Mean Absolute Error (MAE): Shows average prediction error.
Best Model
Random Forest with an R² of 0.96 and RMSE of 1.26.
Optimization
Hyperparameter tuning using GridSearchCV:

Tuned parameters:
n_estimators (number of trees)
max_features (number of features considered at each split)
Final Configuration:
30 trees
Maximum of 8 features
Achieved improved performance and accuracy.
Results
The model's predictions closely matched actual player ratings, validating its accuracy.
Example:
Actual Rating: 69 → Predicted Rating: 69.63
Actual Rating: 75 → Predicted Rating: 75.73
Installation and Usage
Requirements
Python 3.7 or higher
Libraries:
pandas
numpy
matplotlib
seaborn
scikit-learn
