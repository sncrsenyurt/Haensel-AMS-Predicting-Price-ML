# Haensel-AMS-Predicting-Price-ML



# Predicting Price

## Introduction
This data project is a take-home assignment used in the recruitment process for data science positions at Haensel AMS. The goal is to predict the target variable `price` using the provided dataset with 7 attributes.

## Assignment
1. **Data Analysis**: Conduct initial data analysis to understand the structure and connections between attributes.
2. **Model Selection**: Fit one or more ML models and explain the choices.
3. **Model Validation**: Use cross-validation to evaluate the model's performance and comment on the results.
4. **Results Presentation**: Present the results, the steps taken, and provide critical thinking on the next steps.

## Data Description
The data is provided in the `sample.csv` file and includes the following columns:
- loc1
- loc2
- para1
- dow
- para2
- para3
- para4
- price (target variable)

## Practicalities
- **Objective**: Define, train, and evaluate a predictive model for the given data.
- **Data Split**: Split the data into training, testing, and validation sets as needed.
- **External Data**: Do not use external data.
- **Algorithms**: Use any algorithm of choice and compare multiple models if necessary.
- **Time Limit**: Spend no more than 4 hours on this project.
- **Code Structure**: Emphasize code structure and the thought process over final metrics.

## Project Steps

### 1. Data Import and Initial Exploration
- Import necessary libraries and load the dataset.
- Perform basic data exploration to understand the data types and structure.

### 2. Data Cleaning and Manipulation
- Remove rows with invalid entries in `loc1`.
- Convert `loc1` and `loc2` to numeric values.
- Handle missing values.
- Convert the `dow` (day of the week) to numeric values and create dummy variables.

### 3. Feature Selection
- Calculate the correlation matrix to understand the relationship between features and the target variable.
- Select the top features based on correlation for model training.

### 4. Model Training and Evaluation
- Define feature sets for training (full dataset and top features).
- Train multiple regression models (Ridge, DecisionTree, RandomForest, XGBoost, LGBM, MLP).
- Evaluate models using cross-validation and calculate train and test errors, and R-squared values.

### 5. Hyperparameter Tuning with Grid Search
- Perform grid search on the RandomForest model to find the best hyperparameters.
- Train the model with the best parameters and evaluate its performance.

### 6. Scaling
- Apply Min-Max Scaling, Standard Scaling, and Robust Scaling.
- Train the RandomForest model on scaled data and evaluate performance.

### 7. Model Evaluation Summary
- Collect results from different models and scaling techniques.
- Create visualizations to compare the performance of different models and techniques.

## Instructions for Running the Project
1. **Download the Dataset**: Ensure the `sample.csv` file is in the project directory.
2. **Install Required Libraries**: Use `pip` to install the necessary libraries.
   ```bash
   pip install pandas numpy matplotlib scikit-learn xgboost lightgbm
3. **Run the Jupyter Notebook: Open and execute the notebook to follow the steps and reproduce the results.

## Code Structure
The code is structured into sections corresponding to the project steps. Each section includes:
- **Code**: Implementing the necessary functionality.
- **Comments**: Explaining the thought process and the steps taken.

## Conclusion
This project demonstrates the end-to-end process of building a predictive model for the given dataset, from data cleaning and feature selection to model training, hyperparameter tuning, and evaluation. The focus is on the entire workflow and the structured approach rather than just the final model performance.

This project was done as a personal development exercise to improve my skills in data analysis and machine learning.

For any questions or further discussions, please feel free to reach out.
