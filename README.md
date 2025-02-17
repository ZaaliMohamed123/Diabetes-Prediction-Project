# **Diabetes Prediction Project**

This project aims to predict whether a patient has diabetes based on diagnostic measurements. The dataset, sourced from the National Institute of Diabetes and Digestive and Kidney Diseases, contains medical predictor variables such as the number of pregnancies, BMI, insulin level, age, among others. The dataset includes only female patients who are at least 21 years old and of Pima Indian heritage.

**Overview of the Process**

1. Data Collection and Analysis:

 * Loaded the dataset and explored its structure and summary statistics.
 * Identified class imbalance in the target variable, with more non-diabetic than diabetic instances.

2. Handling Imbalanced Dataset:

 * Used under-sampling to balance the dataset by randomly selecting an equal number of non-diabetic samples as there are diabetic samples.

3. Data Preprocessing:

 * Separated features (X) and labels (Y).
 * Standardized the features using StandardScaler to ensure all variables have a mean of 0 and a standard deviation of 1.

4. Parameter Selection with GridSearchCV:

 * Utilized GridSearchCV to find the best hyperparameters for the SVM classifier.

5. Model Training:

 * Split the dataset into training and testing sets using with stratification.
 * Trained an SVM classifier with the best parameters.

6. Model Evaluation:

 * Evaluated the model's performance, achieving training accuracy of 77.71% and test accuracy of 75.32%.

7. Predictive System:

 * Implemented a predictive function that takes input data, preprocesses it, and uses the trained model to predict whether a person is diabetic or not.
