
#  Task 1

Link for this task can be found and followed here: [here](https://github.com/sarora/CodeChallenge/blob/master/CodingChallenge/Data%20Science/Task1.ipynb)


### Key Points and Tasks

1. The target variable was engineered to predict failure between 0 and 40 days.

2. No multiple failures for turbines.

3. Handled missing data through multiple imputation (MICE). Categorical data encoded using `pd.getdummies()`

4. No right censorship in the data. Every machine fails.

5. In this case, I think the cost for checking failures in wind turbines should be lower than cost for failing to check for failures. We can tolerate false positives more. Hence, recall as a metric is used.

6. Performed hyperparameter optimization using `RandomizeSearchCV`.  Used Random Forest Classifier that gave me the highest recall accuracy.

7. **Improvements**: Use over-sampling to balance the dataset more but that could introduces a lot of false-positives. I did not try this.

8. **Improvements**: Use Survival analysis with decision trees.

9. Model saved in the pickle format saved in model folder.

# Task 2

Link for this notebook can be found [here](https://github.com/sarora/CodeChallenge/blob/master/CodingChallenge/Data%20Science/Task2.ipynb)

Link for this notebook using Keras NN can be found [here](https://github.com/sarora/CodeChallenge/blob/master/CodingChallenge/Data%20Science/Task2_NN.ipynb)



### Key Points and Tasks


1. The target variable was engineered to predict 6 hours ahead.

2.  Handled missing data through multiple imputation (MICE). categorical data using `pd.getdummies()`

3. Compared various sklearn regression models. Model selected  is `RandomForestRegressor`.

4. Metrics used were $R^2$ along with root mean square error to evaluate model performance.

5.  Performed hyperparameter optimization using `RandomizeSearchCV`.`

6. Perform feature selection using `Lasso` to improve performnace.

7. Used Neural Networks to "improve" the performance of Random Forest Model.

8. Model saved in the pickle format saved in model folder.

9. **Improvements/Future work**: Use PCA for feature selection. Reduce dimensionality/features.

10. **Improvements/Future work**: Hypertune keras neural network
