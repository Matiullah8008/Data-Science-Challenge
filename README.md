# Data Science Coding Challenge: Churn Prediction

## Project Overview

This project is a solution to a data science coding challenge focused on predicting customer churn for a video streaming service. The goal is to build a machine learning model that can identify existing subscribers who are likely to cancel their subscriptions in the upcoming month.

## Dataset

The dataset consists of two files: `train.csv` and `test.csv`.

*   `train.csv`: Contains historical subscription data, including features about the customer, their streaming preferences, activity, and a `Churn` column indicating whether the subscriber churned (1) or not (0). This dataset is used for training the model.
*   `test.csv`: Contains similar information as `train.csv` but without the `Churn` column. This dataset is used for making predictions.

The `data_descriptions.csv` file provides a detailed description of each column in the dataset.

## Project Steps

The notebook follows these key steps:

1.  **Import Libraries**: Import necessary Python libraries for data manipulation, machine learning, and visualization.
2.  **Load Data**: Load the `train.csv` and `test.csv` files into pandas DataFrames.
3.  **Explore, Clean, Validate, and Visualize Data**: Perform initial data analysis to understand the data distribution, identify missing values, and visualize relationships between features and the target variable. This includes:
    *   Checking data types and missing values.
    *   Displaying descriptive statistics.
    *   Visualizing feature distributions and relationships with churn (e.g., Account Age, Monthly Charges, Subscription Type, Payment Method).
4.  **Handle Missing Values**: Address any missing values in the datasets using appropriate strategies (e.g., filling with mode or mean).
5.  **Feature Engineering**: Create new features or transform existing ones to potentially improve model performance. An example created is `ChargesPerMonth`.
6.  **Preprocess Categorical Features**: Convert categorical features into a numerical format using techniques like one-hot encoding.
7.  **Select and Train a Model**: Choose a suitable classification model (e.g., RandomForestClassifier, GradientBoostingClassifier, LogisticRegression) and train it on the preprocessed training data. The notebook includes options to experiment with different algorithms and apply hyperparameter tuning results.
8.  **Make Predictions**: Use the trained model to predict the churn probabilities for the test dataset.
9.  **Create Submission File**: Generate a `prediction_df` DataFrame with `CustomerID` and `predicted_probability` columns in the required format for submission.
10. **Final Tests**: Run assertion tests to verify the structure and format of the submission file.

## How to Run the Notebook

1.  Ensure you have the necessary data files (`train.csv`, `test.csv`, `data_descriptions.csv`) in the correct location.
2.  Open the notebook in a compatible environment (like Google Colab).
3.  Run each cell sequentially from top to bottom.
4.  Review the output of each cell to understand the data and the steps being performed.
5.  Experiment with different feature engineering techniques, preprocessing steps, and machine learning models to potentially improve your prediction score.
6.  After making predictions and creating the `prediction_df`, run the final test cells to validate the submission format.
7.  Save the `prediction_df` to a CSV file named `prediction_submission.csv`.
8.  Submit the `prediction_submission.csv` file according to the competition instructions.

## Requirements

The notebook primarily uses the following Python libraries:

*   pandas
*   numpy
*   scikit-learn
*   matplotlib
*   seaborn

Ensure these libraries are installed in your environment. In Google Colab, most of these are pre-installed.

## Authors

*   [Matiullah] - *Initial work*

---
