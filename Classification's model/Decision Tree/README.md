# Decision Tree Classification

This directory contains a comprehensive implementation of the Decision Tree algorithm for binary classification using the Social Network Ads dataset.

## Overview

Decision Tree is a non-parametric supervised learning algorithm that creates a tree-like model of decisions. It splits the data recursively based on feature values to create the most homogeneous subsets, making it highly interpretable and effective for both classification and regression tasks.

## Files

- `decision_tree.ipynb` - Complete Jupyter notebook with Decision Tree implementation
- `Social_Network_Ads.csv` - Dataset containing user information (Age, EstimatedSalary, Purchased)
- `README.md` - This file

## Dataset

The Social Network Ads dataset contains:
- **Age**: User's age (continuous variable)
- **EstimatedSalary**: User's estimated salary (continuous variable)
- **Purchased**: Whether the user purchased the product (0 = No, 1 = Yes)

## What You'll Learn

### Core Concepts
1. **Decision Tree Structure**: Understanding nodes, leaves, and splits
2. **Splitting Criteria**: Gini impurity vs Entropy
3. **Recursive Partitioning**: How trees grow through data splitting
4. **Pruning Techniques**: Preventing overfitting with constraints

### Implementation Features
1. **Multiple Model Variations**: Default, depth-constrained, and sample-constrained trees
2. **Hyperparameter Tuning**: GridSearchCV for optimal parameters
3. **Overfitting Analysis**: Training vs test accuracy comparison
4. **Feature Importance**: Understanding which features matter most

### Advanced Analysis
1. **Tree Visualization**: Graphical representation of decision rules
2. **Decision Boundary Plots**: Visual understanding of classification regions
3. **Cross-Validation**: Model stability assessment
4. **Algorithm Comparison**: Performance vs K-NN and Naive Bayes

## Key Features

### Comprehensive Model Training
- **Default Decision Tree**: Unrestricted tree growth
- **Max Depth Constraint**: Limiting tree depth (max_depth=5)
- **Minimum Samples Constraint**: Controlling leaf size (min_samples_leaf=10)
- **No Scaling Model**: Demonstrating scale independence

### Advanced Evaluation
- **Multiple Metrics**: Accuracy, precision, recall, F1-score
- **Confusion Matrices**: Visual classification breakdown
- **ROC Curves**: Performance across different thresholds
- **Cross-Validation**: 10-fold validation for stability

### Visualization Suite
- **Tree Structure**: Complete decision tree visualization
- **Feature Importance**: Bar charts showing feature contributions
- **Decision Boundaries**: 2D visualization of classification regions
- **Overfitting Analysis**: Training vs test accuracy curves

### Hyperparameter Optimization
- **Grid Search**: Systematic parameter exploration
- **Parameter Analysis**: Impact of different constraints
- **Best Model Selection**: Optimal configuration identification

## Mathematical Foundation

### Splitting Criteria

**Gini Impurity**: 
```
Gini = 1 - Σ(pi)²
```
Where pi is the probability of class i

**Entropy**:
```
Entropy = -Σ(pi × log2(pi))
```

**Information Gain**:
```
IG = Entropy(parent) - Σ(weight × Entropy(child))
```

## Model Performance

The Decision Tree models demonstrate:
- **High Interpretability**: Clear decision rules
- **Good Accuracy**: Competitive with other algorithms
- **Feature Insights**: Automatic feature importance ranking
- **Flexible Decision Boundaries**: Non-linear classification capability

## Advantages and Disadvantages

### Advantages
✅ **Highly Interpretable**: Easy to understand decision rules
✅ **No Feature Scaling Required**: Works with raw data
✅ **Handles Non-linear Relationships**: Captures complex patterns
✅ **Automatic Feature Selection**: Identifies important features
✅ **Mixed Data Types**: Handles numerical and categorical data
✅ **No Statistical Assumptions**: Distribution-free approach

### Disadvantages
❌ **Overfitting Prone**: Can create overly complex trees
❌ **Instability**: Sensitive to small data changes
❌ **Feature Bias**: May favor features with more categories
❌ **Limited Linear Relationships**: May overfit simple patterns
❌ **Greedy Algorithm**: May not find globally optimal tree

## Best Practices

### Parameter Tuning
1. **max_depth**: Start with 3-10, increase if underfitting
2. **min_samples_split**: Use 2-20, higher for larger datasets
3. **min_samples_leaf**: Use 1-10, higher to prevent overfitting
4. **criterion**: 'gini' for speed, 'entropy' for potential accuracy gain

### Overfitting Prevention
1. **Pruning**: Use max_depth, min_samples constraints
2. **Cross-Validation**: Validate performance stability
3. **Ensemble Methods**: Consider Random Forest for better generalization
4. **Feature Engineering**: Remove irrelevant or redundant features

## Real-World Applications

Decision Trees excel in:
- **Healthcare**: Medical diagnosis and treatment decisions
- **Finance**: Credit scoring and risk assessment
- **Marketing**: Customer segmentation and targeting
- **Business**: Rule-based decision systems
- **Manufacturing**: Quality control and process optimization

## Getting Started

### Prerequisites
```python
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Quick Start
1. Open `decision_tree.ipynb` in Jupyter Notebook or VS Code
2. Run all cells to see the complete implementation
3. Experiment with different parameters in the hyperparameter tuning section
4. Modify the visualization functions to explore your own datasets

### Customization
- **Different Datasets**: Replace the CSV file and adjust feature names
- **Multi-class Classification**: Extend to more than 2 classes
- **Regression**: Use DecisionTreeRegressor for continuous targets
- **Ensemble**: Combine with Random Forest or Gradient Boosting

## Comparison with Other Algorithms

| Algorithm | Interpretability | Accuracy | Speed | Overfitting Risk |
|-----------|-----------------|----------|-------|------------------|
| Decision Tree | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ |
| K-NN | ⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ |
| Naive Bayes | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |

## Future Enhancements

Consider exploring:
- **Random Forest**: Ensemble of decision trees
- **Gradient Boosting**: Sequential tree improvement
- **XGBoost**: Advanced gradient boosting
- **Feature Engineering**: Creating new meaningful features
- **Pruning Algorithms**: Post-pruning techniques

This implementation provides a solid foundation for understanding and applying Decision Tree classification in real-world scenarios.
