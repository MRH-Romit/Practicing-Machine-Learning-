# K-Nearest Neighbors (K-NN) Analysis

This folder contains my practice work on K-Nearest Neighbors algorithm for classification problems.

## Dataset

- **File**: `Social_Network_Ads.csv`
- **Description**: A dataset containing user information (Age, Estimated Salary) and whether they purchased a product (1) or not (0).

## Implementation

- **File**: `k_nearest_neighbors.ipynb`
- **Description**: A Jupyter Notebook implementing K-Nearest Neighbors to predict purchase decisions based on age and estimated salary.

## Summary of K-Nearest Neighbors (K-NN)

### 🔍 Key Idea:

- K-NN is a **non-parametric**, **instance-based** learning algorithm.
- It makes predictions based on the **k** most similar instances in the training dataset.

🔸 **K-Nearest Neighbors**:

- A simple, versatile classification algorithm.
- Makes predictions based on the majority class of the k nearest neighbors.
- No explicit training phase - it "memorizes" the training data.

🔸 **When to Use**:

- For small to medium-sized datasets.
- When you need a simple baseline model.
- When interpretability is important.
- For problems where proximity in feature space correlates with similarity in outcomes.

🔸 **Key Concepts**:

- **K Value**: The number of neighbors to consider (hyperparameter).
- **Distance Metric**: How to measure similarity between instances (commonly Euclidean distance).
- **Majority Voting**: The final prediction is determined by the most common class among neighbors.

🔸 **Advantages**:

- Simple to understand and implement.
- No assumptions about data distribution.
- Effective for multi-class problems.
- Can be used for both classification and regression.

🔸 **Disadvantages**:

- Computationally expensive for large datasets.
- Sensitive to irrelevant features and the scale of the data.
- Requires feature scaling.
- Curse of dimensionality affects performance in high-dimensional spaces.

## Results

- Implemented K-NN classifier using scikit-learn with k=5 and Minkowski distance.
- Achieved classification accuracy measured with confusion matrix.
- Visualized decision boundaries for both training and test sets.
- Predicted purchase decisions for new customer data.
