# Challenge A – Boston Housing Price Prediction (Weka)

This project demonstrates the use of **Weka** to build a predictive model for house prices using the **Boston Housing dataset** as part of **Module 4 – Machine Learning**.

---

## Dataset
The Boston Housing dataset contains **506 instances** with numeric attributes describing housing, environmental, and socio-economic factors.  
The target variable is **MEDV**, representing the median value of owner-occupied homes.

---

## Data Preparation
1. The dataset was loaded into **Weka Explorer**.
2. An index column was identified and removed as it did not provide predictive value.
3. All remaining attributes were numeric, so no encoding was required.
4. The target variable was set to **MEDV**.

---

## Algorithms Tested
The following regression algorithms were evaluated using **10-fold cross-validation**:
- SMOreg  
- MultilayerPerceptron  
- RandomForest  

Performance was compared using correlation coefficient, mean absolute error (MAE), and root mean squared error (RMSE).

---

## Final Model Selection
**RandomForest regression** produced the best performance and was selected as the final model.

### Key Settings:
- Number of trees (numIterations): **500**
- Maximum depth: **Unlimited**
- Evaluation method: **10-fold cross-validation**

---

## Results
The final RandomForest model achieved the following performance:

- **Correlation coefficient:** 0.9392  
- **Mean absolute error:** 2.1417  
- **Root mean squared error:** 3.2406  
- **Total instances:** 506  

These results indicate strong predictive performance for estimating house prices.

---

## Screenshots

### RandomForest Configuration
![RandomForest Parameters](img/randomforest_parameters.png)

### Model Performance Output
![RandomForest Results](img/randomforest_results.png)

---

## Conclusion
RandomForest regression provided the most accurate and stable predictions compared to the other algorithms tested. This confirms its suitability for modelling complex, non-linear relationships in the Boston Housing dataset.

---

## Author
**Derrick Ahortu**  
Module 4 – Machine Learning
