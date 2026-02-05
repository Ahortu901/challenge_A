Challenge A (Weka) – Step-by-Step Data Filtering and Algorithm Testing
Step 1: Load the dataset

The Boston Housing dataset was opened in Weka Explorer using the Preprocess tab. The dataset contained 506 instances and a range of numeric attributes describing housing, environmental, and socio-economic factors.

Step 2: Filter the data

An index column was identified in the dataset and removed using the Remove attribute filter, as it did not contain any predictive information and only represented row numbering.

No further filtering or encoding was required because all remaining attributes were numeric and suitable for regression analysis.

Step 3: Select the target variable

In the Classify tab, the target variable was set to MEDV, which represents the median value of owner-occupied homes. This configured the task as a regression problem.

Step 4: Choose evaluation method

The evaluation method was set to 10-fold cross-validation to provide a reliable estimate of model performance across the full dataset.

Step 5: Algorithms tested

Several regression algorithms were tested and compared using Weka, including:

SMOreg

MultilayerPerceptron

RandomForest

Performance was compared using Weka’s regression metrics, including correlation coefficient, mean absolute error, and root mean squared error.

Step 6: Final algorithm and settings

RandomForest was selected as the final model due to superior performance.

The following settings were used (as shown in the screenshot):

Number of trees (numIterations): 500

Maximum depth: Unlimited

All other parameters left at default values

10-fold cross-validation

Step 7: Results

The final RandomForest model achieved the following performance:

Correlation coefficient: 0.9392

Mean absolute error: 2.1417

Root mean squared error: 3.2406

Total instances: 506

These results demonstrate strong predictive performance for house price estimation.

Step 8: Conclusion

RandomForest regression provided the best balance of accuracy and robustness compared to the other algorithms tested. The model was therefore selected as the final solution for predicting house prices in the Boston Housing dataset.
