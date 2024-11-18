# Thyroid Disease Classification Using Machine Learning

This project classifies thyroid disease based on health-related attributes using machine learning. The goal is to predict whether a patient has a thyroid disorder (`P` for positive) or not (`N` for negative). The models applied are **Logistic Regression**, **Random Forest**, and **Support Vector Machine (SVM)**.

## Steps Involved

### 1. **Data Preprocessing**
   - Cleaned the dataset and encoded categorical features.
   - Addressed missing values and scaled numerical features for model compatibility.
   
### 2. **Model Training and Evaluation**
   - Three models were trained: Logistic Regression, Random Forest, and SVM.
   - Evaluated using **accuracy**, **precision**, **recall**, and **F1-score**.

### 3. **Model Comparison**
   - All models performed similarly with accuracies around **91-92%**.
   - Struggled with predicting the negative class (`N`) due to class imbalance.

## Results

### Logistic Regression
   - **Accuracy**: 92.32%
   - High performance for the positive class but struggled with the negative class (`N`).
   - **Precision**: 0.92 for `P`, 0.00 for `N`

### Random Forest
   - **Accuracy**: 91.52%
   - Similar to Logistic Regression, performed well for positive class.
   - **Precision**: 0.92 for `P`, 0.00 for `N`

### Support Vector Machine (SVM)
   - **Accuracy**: 91.92%
   - Similar pattern: high precision for the positive class, low for the negative class.
   - **Precision**: 0.92 for `P`, 0.00 for `N`

## Insights
- All models performed well for the positive class (`P`) but struggled with the negative class (`N`), indicating class imbalance.
- **Class Imbalance**: The poor predictions for the negative class suggest further steps are needed to handle imbalance.

## Next Steps
- Implement **SMOTE** or **adjust class weights** to address class imbalance.
- Tune model hyperparameters using **GridSearchCV** or **RandomizedSearchCV**.
- Explore ensemble methods like **Voting Classifiers** for improved performance.

## Visualizations
- **Accuracy Comparison**: Bar charts for model accuracy.
- **Precision-Recall Curves** and **Confusion Matrices** to evaluate model performance on imbalanced data.

## Conclusion
This project demonstrates the application of machine learning for thyroid disease classification. Future work includes handling class imbalance and optimizing models for better overall performance.


