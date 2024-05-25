# Salary Prediction using Polynomial Regression

## Author
Eric Ramirez

## Purpose
The goal of this script is to accurately predict the salary of a potential employee who is asking for a salary of $160,000. He claims that this was his previous salary, and his LinkedIn profile indicates he is a Regional Manager with 2 years of experience. This positions him between a Regional Manager and a Partner in our dataset. The hiring manager wants to use this model to analyze if his requested salary is above or below the market value, aiding in salary negotiations.

## Dataset
The dataset used in this analysis contains the following information:
- Position
- Level
- Salary

## Machine Learning Strategies
To achieve accurate predictions and better fit the salary data, we employ the following machine learning strategies:
1. **Linear Regression**: A simple model that assumes a linear relationship between the position level and the salary. This model helps provide a baseline for comparison.
2. **Polynomial Regression**: An extension of linear regression where we fit a polynomial to the data instead of a straight line. This model is more flexible and can capture the nonlinear relationships in the data, providing a more accurate fit.

## Code Overview

### Libraries
The following libraries are used:
- `numpy`
- `matplotlib`
- `pandas`
- `sklearn.linear_model`
- `sklearn.preprocessing`

### Steps
1. **Importing the Dataset**: Load the dataset and extract the features (Position Level) and target variable (Salary).
2. **Training the Linear Regression Model**: Fit a linear regression model to the entire dataset.
3. **Training the Polynomial Regression Model**: Transform the features and fit a polynomial regression model to the entire dataset with a degree of 4.
4. **Visualization**: Visualize both models to see the fit on the dataset.
5. **Prediction**: Predict the salary for a Regional Manager with 2 years of experience using both models.

### Visualizations
#### Linear Regression Model
![linear_regression](https://github.com/Akira6713/salary-prediciton-BI/assets/66973202/5a5e7139-251e-4ce5-b9f9-8f0c8e764e7c)

#### Polynomial Regression Model
![polynomial_regression](https://github.com/Akira6713/salary-prediciton-BI/assets/66973202/1d192b7e-aa2f-4c33-8e74-6c608ed2e62f)

### Predictions
- **Linear Regression prediction for Regional Manager w/ 2 years experience**:  $330,378.79
- **Polynomial Regression prediction for Regional Manager w/ 2 years experience**:  $158,862.45

## Output
## Interpretation
The Linear Regression model predicts a salary of approximately $330,378.79, which is significantly higher than the requested salary of $160,000. On the other hand, the Polynomial Regression model predicts a salary of approximately $158,862.45, which is very close to the requested salary.

## Usage for Salary Negotiation
The hiring manager can use these predictions to negotiate the salary with the potential employee. Since the Polynomial Regression model provides a more accurate fit to the dataset, its prediction of $158,862.45 suggests that the requested salary of $160,000 is reasonable and aligns with market expectations for a Regional Manager with 2 years of experience.

## Conclusion
From the dataset and our analysis, it is evident that the Polynomial Regression model fits the data more accurately compared to the Linear Regression model. The prediction of $158,862.45 by the Polynomial Regression model closely matches the requested salary of $160,000, indicating that the candidate's request is fair and within the expected range for a Regional Manager with 2 years of experience. The hiring manager can confidently use this model to negotiate the salary, ensuring that it is aligned with market standards.
