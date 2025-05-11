# Logistic Regression Analysis

This folder contains my practice work on Logistic Regression for classification problems.

## Dataset

- **File**: `Social_Network_Ads.csv`
- **Description**: A dataset containing user information (Age, Estimated Salary) and whether they purchased a product (1) or not (0).

## Implementation

- **File**: `logistic_regression.ipynb`
- **Description**: A Jupyter Notebook implementing Logistic Regression to predict purchase decisions based on age and estimated salary.

## Summary of Logistic Regression

### 🔍 Key Idea:

- **Regression** usually means predicting a number (like predicting a salary).
- But **logistic regression** is different:
    
    ➤ It predicts the **probability** of a class (like pass/fail).
    
    ➤ Then, it **converts** that probability into a **category** (class).
    
    🔸 **Logistic Regression**:
    
    - A classification algorithm in machine learning.
    - Predicts the probability of an outcome belonging to a specific class (e.g., Yes/No, Pass/Fail, 1/0).
    - Uses a sigmoid function to map predictions between 0 and 1.
    
    🔸 **When to Use**:
    
    - For problems with categorical outcomes (binary or multi-class).
    - Examples: Spam detection, Disease diagnosis, Win/Loss prediction.
    
    🔸 **Key Concepts**:
    
    - Sigmoid Function: Maps any real number into a probability (0 to 1).
    - Threshold: Assigns class 1 if probability > 0.5, class 0 otherwise.
    
    🔸 **Formula**:
    
    - Linear part: z = w₁x₁ + w₂x₂ + ... + b
    - Sigmoid: σ(z) = 1 / (1 + e^(-z))
    - Output: Probability of the class

## Results

- Implemented logistic regression classifier using scikit-learn
- Achieved classification accuracy measured with confusion matrix
- Visualized decision boundaries for both training and test sets
- Predicted purchase decisions for new customer data
