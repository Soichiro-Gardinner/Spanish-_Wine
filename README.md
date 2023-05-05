# Wine Acidity Prediction

Business Problem and Stakeholders
A wine company wants to optimize the acidity levels of their wines. They want to know the acidity level that makes their wines the most enjoyable to their customers. The stakeholders are the company executives who make business decisions based on the wine acidity prediction models.

# Data Source
- Kaggle

# Data Description
The dataset contains 1599 observations and 12 features, including the wine's fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulphates, alcohol content, and quality. The quality column is the target variable, and it is a measure of the wine's overall quality.

# Analytical Insights
## Correlation Heat-Map:
![alt text](https://user-images.githubusercontent.com/124306090/236449338-aec55001-b8dc-4919-9204-73ebacec98b3.png)
- we can see that there is a moderate positive correlation between price and rating, indicating that higher-priced wines tend to have higher ratings. This can be an insight for the stakeholder to consider when pricing their wines.


# "Predicting Wine Acidity and Quality Using Machine Learning: A Random Forest Approach with Hyperparameter Tuning
The pH level of wines shows a moderate correlation with their quality. Lower pH levels are associated with higher-quality wines.
Wines with higher alcohol content generally have better quality ratings.
Model Performance
The random forest model with hyperparameters {'max_depth': 15, 'n_estimators': 100} had the best performance, with a test RMSE of 0.239 and test R^2 of 0.463. This model could predict the acidity levels of wines to optimize their taste and quality.

### Why Is it important to predict wine's acidity?
![alt text](https://user-images.githubusercontent.com/124306090/236453402-43674a52-8de7-4ff7-b376-d57e621f503e.png)
- **Because:** From the line plot, we can see that there is a moderate negative correlation between acidity and quality ratings. As the acidity level increases, the quality ratings tend to decrease.


# Model Recommendations
The company should aim to produce wines with lower pH levels to improve their quality.
The company should also produce wines with higher alcohol content, which are generally rated higher in quality.

## Work Committed:

- Feature Engineering: A loop was created to detect any values with the string "N.V." in the 'year' column and replace them with the mode of the column.

- Modeling: Multiple types of models were trained and evaluated on the dataset. The models included Linear Regression, Lasso, Ridge, Decision Tree, and Random Forest. The models were tuned using GridSearchCV to optimize their hyperparameters. The models were evaluated on both the training and testing datasets using various metrics such as RMSE and R^2.

- Production Model: The Random Forest model was selected as the production model based on its performance metrics. It had the lowest test RMSE and the highest test R^2 score among all the models tested.
