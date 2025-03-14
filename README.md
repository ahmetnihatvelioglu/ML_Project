# ML_Project

## Overview
This repository contains a Jupyter notebook implementing various machine learning algorithms for data analysis and prediction. The project demonstrates the application of machine learning techniques to solve real-world problems through data preprocessing, model training, and evaluation.

## Installation
**To run this project, you'll need Python and several libraries. You can install the required dependencies using:**

"pip install -r requirements.txt"

**Alternatively, you can install the following packages individually:**

"pip install numpy pandas matplotlib seaborn scikit-learn jupyter"

## Features
**Data Preprocessing**: Handling missing values, feature scaling, and encoding categorical variables

**Exploratory Data Analysis**: Visualizing data distributions and correlations

**Feature Engineering**: Creating new features to improve model performance

**Model Selection**: Comparing multiple machine learning algorithms

**Hyperparameter Tuning**: Optimizing model parameters for better results

**Model Evaluation**: Using various metrics to assess model performance

## Models

The following machine learning models were implemented and evaluated:

- Linear Regression

- Decision Trees


## Results

In this project, Forest Fire Index (FWI) was estimated using Algerian forest fires dataset. Our aim is to accurately estimate the FWI value by analyzing the environmental factors affecting fire risk. In this direction, multiple linear regression and decision tree regression models were trained and their performances were compared.

### Data Preprocessing and Key Findings:

- The dataset was subjected to various pre-processing steps such as cleaning missing values ​​and converting categorical variables to numerical format.

- Correlation analysis revealed the relationships between the features and identified the key factors associated with FWI.

- Feature Engineering:

  The columns 'day', 'month' and 'year' were removed as they were unnecessary for the analysis.

  Categorical columns were converted to numerical data.

### Model Performance:

**Multiple Linear Regression:**

- MSE: 0.3554 and R²: 0.9883 values ​​were obtained in the test dataset. This shows that the model can predict the FWI value with high accuracy.

- The MSE value obtained with Cross-Validation was found to be 2.3056, which supports the good overall performance of the model.

- Statistical significance tests (OLS model summary) showed that the model was generally significant, but it was determined that some independent variables (e.g., 'temperature', 'rh', 'ws') did not make statistically significant contributions.

- Confidence interval analysis showed how accurate the model's predictions were at a certain confidence level.

**Decision Tree Regression:**

- MSE: 2.2878 and R²: 0.9245 values ​​were obtained in the test dataset. This indicates a lower performance compared to multiple linear regression.

- The MSE value obtained by cross-validation was found to be 3.6692, which suggests that the model tends to overfit.

- While it shows excellent performance on the training data (MSE: 0.0000, R²: 1.0000), it shows a lower performance on the test data, indicating an overfitting problem.

- The feature importance analysis showed that features such as 'isi' and 'bui' are the most effective factors on the FWI estimation.


### Model Comparison and Interpretation of Results:

- The multiple linear regression model showed better overall performance than the decision tree regression.

- Error distribution plots showed the distribution of prediction errors for both models and provided information about the strengths and weaknesses of the models.

- Comparison of the actual and predicted FWI values ​​provided the opportunity to visually evaluate the prediction accuracy of the models.



























