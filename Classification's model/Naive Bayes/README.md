# Naive Bayes Classification

This directory contains a complete implementation of the Naive Bayes algorithm for binary classification using the Social Network Ads dataset.

## Overview

Naive Bayes is a probabilistic classification algorithm based on Bayes' theorem with the "naive" assumption that features are independent of each other. Despite this strong assumption, it often performs surprisingly well in practice.

## Files

- `naive_bayes.ipynb` - Complete Jupyter notebook with Naive Bayes implementation
- `Social_Network_Ads.csv` - Dataset containing user information (Age, EstimatedSalary, Purchased)
- `README.md` - This file

## Dataset

The Social Network Ads dataset contains:
- **Age**: User's age
- **EstimatedSalary**: User's estimated salary
- **Purchased**: Whether the user purchased the product (0 = No, 1 = Yes)

## What You'll Learn

1. **Bayes' Theorem**: Understanding the mathematical foundation
2. **Gaussian Naive Bayes**: Implementation for continuous features
3. **Feature Independence**: The "naive" assumption and its implications
4. **Model Evaluation**: Comprehensive performance analysis
5. **Visualization**: Decision boundaries and feature relationships
6. **Comparison**: Performance comparison with K-NN algorithm

## Key Features

- Complete data preprocessing pipeline
- Feature scaling and train/test split
- Gaussian Naive Bayes implementation
- Comprehensive model evaluation (confusion matrix, accuracy, classification report, ROC curve)
- Beautiful visualizations of decision boundaries
- Analysis of the independence assumption
- Comparison with K-NN performance
- Probability predictions with confidence levels

## Mathematical Foundation

The algorithm applies Bayes' theorem:

**P(class|features) = P(features|class) × P(class) / P(features)**

Where:
- P(class|features): Posterior probability
- P(features|class): Likelihood
- P(class): Prior probability
- P(features): Evidence

## Results

The Naive Bayes model achieves excellent performance on this dataset, demonstrating:
- High accuracy in binary classification
- Good separation of classes in the feature space
- Robust probability estimates
- Competitive performance compared to K-NN

## When to Use Naive Bayes

- Limited training data available
- Need for fast training and prediction
- Probability estimates required
- Features are approximately independent
- Text classification tasks
- Spam detection
- Medical diagnosis

## Getting Started

1. Ensure you have the required libraries: `numpy`, `pandas`, `matplotlib`, `sklearn`, `seaborn`
2. Open `naive_bayes.ipynb` in Jupyter Notebook or VS Code
3. Run all cells to see the complete implementation and results

The notebook is well-documented with explanations of each step and the mathematical concepts behind Naive Bayes classification.
