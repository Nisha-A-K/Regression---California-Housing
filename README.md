# California Housing Data Analysis
This project focuses on analyzing and predicting housing prices in California using the California Housing Dataset. The dataset contains information about various attributes of districts in California, such as average income, housing age, number of rooms, and geographic location, which are used to predict the median house value for the district.

## Table of Contents
1. Project Overview
2. Dataset
3. Installation. 
4. Data Preprocessing
5. Modeling
6. Evaluation

   
## Project Overview
The goal of this project is to explore the California Housing Dataset and build machine learning models to predict the median house value for each district. This analysis involves data cleaning, exploratory data analysis (EDA), feature engineering, and building regression models such as Decision Trees, Random Forest, AdaBoost, and other algorithms.

## Dataset
The California Housing Dataset used in this project  contains the following columns:

1. MedInc: Median income of the district.
2. HouseAge: Median age of houses in the district.
3. AveRooms: Average number of rooms per district.
4. AveOccup: Average number of occupants per household.
5. Latitude: Latitude of the district.
6. Longitude: Longitude of the district.
7. Target variable - Median house value for the district.

## Requirements:
Python 3.x
pandas
numpy
scikit-learn
matplotlib
seaborn
jupyterlab (optional for running notebooks)

## Data Preprocessing
The data is first loaded and cleaned to handle any missing values or outliers. The key steps involved in preprocessing are:

## Missing Value Imputation: Handling missing data using strategies such as mean imputation.
1. Feature Scaling: Scaling numerical features using standard scaling techniques.
2. Feature Engineering: Creating new features or transforming existing ones to improve model performance.
3. Train-Test Split: Splitting the dataset into training and testing subsets for evaluation.

## Modeling
Several machine learning models were tested on the dataset:

1. Linear Regression: A baseline model to predict house prices based on linear relationships.
2. Decision Tree Regressor: A model that uses decision rules to predict house prices.
3. Random Forest Regressor: An ensemble method combining multiple decision trees.
4. AdaBoost Regressor: A boosting technique that adjusts weights of incorrectly predicted instances to improve accuracy.
5. Gradient Boosting Regressor: An additive model by combining multiple weak learners (typically decision trees), optimizing for a given loss function to make accurate predictions.
6. MLP Regressor : A neural network-based model that uses multiple layers of neurons to learn non-linear relationships between input features and continuous target values for regression tasks.
   
Each model is evaluated on the test set using metrics like RMSE (Root Mean Squared Error) and R² score.

## Evaluation
The models are evaluated based on the following performance metrics:

1. RMSE (Root Mean Squared Error): Measures the average magnitude of the error in prediction.
2.R² Score: Represents the proportion of variance in the target variable explained by the model.
3. After training and evaluating each model, we compare their performance to determine the best model for predicting median house values.



from sklearn.metrics import mean_squared_error
y_pred = model.predict(X_test)
rmse = np.sqrt(mean_squared_error(y_test, y_pred))
print(f"RMSE: {rmse}")
Contributing
If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. Please ensure that your code follows the project’s style guide and includes tests for new features or bug fixes.
