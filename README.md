# Hi there, I'm Hemang Gautam.

## Overview

This project involves selecting and improving machine learning models for a given dataset. The dataset provided was clean with no null values, and all columns were numeric.

## Data Preprocessing

1. **Variance Threshold**: Dropped columns with variance less than 0.25 to reduce dimensionality.
2. **Standardization**: Standardized the data to ensure equal contribution from all features.

## Model Selection

### Basic Models
- Logistic Regression
- Naive Bayes
- Support Vector Machine (SVM)

### Advanced Models
- XGBoost
- Random Forest Classifier

### Model Performance
The basic models did not yield promising results. Therefore, advanced models were tested, and the XGBoost model performed the best among them.

## Custom Thresholds

To further improve the XGBoost model, custom thresholds were set. A threshold of 0.34 was found to be the most effective. Further, performance was improved using hyperparameter tuning and Cross Validation.

## Ensemble Methods

### Weighted Average
Best weights were found by defining a function that checked F1 scores on various weights.
Combined the results of:
- XGBoost
- Random Forest Classifier
- Logistic Regression
  
### Stacking
Tried stacking multiple models to create a meta-model.

## Best Models

1. **XGBoost with custom threshold of 0.34**
2. **Weighted average of XGBoost, Random Forest Classifier, and Logistic Regression**

## Further Improvements

1. **Feature Engineering**: Create new features based on domain knowledge.
4. **Ensemble Methods**: Explore other ensemble methods like Bagging, Boosting, AdaBoost, or GBM.
5. **Feature Selection**: Use methods like Recursive Feature Elimination (RFE) or feature importances from tree-based models.
6. **Advanced Techniques**: Consider AutoML frameworks (TPOT, AutoKeras) or neural networks for further improvement.

## Conclusion

This project demonstrated the importance of model selection and the effectiveness of advanced models and ensemble methods. The best results were obtained using XGBoost with a custom threshold and a weighted average of multiple models.
