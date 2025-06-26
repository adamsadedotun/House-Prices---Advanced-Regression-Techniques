# House-Prices---Advanced-Regression-Techniques
 House Prices - Advanced Regression Techniques  Welcome to my solution for the Kaggle competition: House Prices - Advanced Regression Techniques. This project applies machine learning to predict the sale prices of houses in Ames, Iowa, based on a dataset of 79 explanatory variables.
 Objective

Build a regression model that predicts the SalePrice of homes using features such as living area, number of rooms, garage size, and more.
The goal is to minimise Root Mean Squared Log Error (RMSLE) between predicted and actual prices.

 Dataset

- Source: Kaggle Competition Link
- train.csv: 1460 rows × 81 columns
- test.csv: 1459 rows × 80 columns
- data_description.txt: Detailed info about each feature

 Preprocessing

- Selected numeric and important categorical features
- Handled missing values using simple imputation (e.g., filling with 0 or the most frequent)
- Applied log transformation to the target variable SalePrice to reduce skew
- Encoded categorical features using one-hot encoding

 Models Used

- RandomForestRegressor: Baseline model with tuned features
- XGBRegressor: Gradient boosting model (better generalisation)
- LGBMRegressor: Fast gradient boosting alternative (optional)

Evaluation

- Training/validation split using train_test_split()
- Used mean_absolute_error and root mean squared error (RMSE) to evaluate
- Submission evaluated using RMSLE on Kaggle

Example Output:
Validation RMSE: 7,623.11
 Submission Format

The output CSV for Kaggle submission follows this format:
Id, SalePrice
1461,169000.1
1462,187724.1233
1463,175221.0

 Future Improvements

- Advanced feature engineering (e.g., polynomial features, interaction terms)
- Hyperparameter tuning using GridSearchCV or Optuna
- Outlier removal
- Ensembling multiple models for better accuracy

Tools & Libraries

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost, LightGBM
- Jupyter Notebook
- Matplotlib / Seaborn (for visualisation)

Author

Adams Adedotun
Portfolio: https://adamsportfolios.netlify.app/
LinkedIn: https://www.linkedin.com/in/adedotun-adams
