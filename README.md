# Bank Marketing Classification

Machine learning classification project for predicting whether a bank customer will subscribe to a term deposit.

## Project Overview
This project compares three classification approaches on an imbalanced bank marketing dataset:
- Logistic Regression
- Decision Tree
- Hard Voting Ensemble

The main goal was to study how model parameters affect classification performance and to identify the most suitable configuration for the dataset.

## Dataset
- 4,521 customer records
- 16 input features
- Binary target: term deposit subscription
- Minority class: approximately 11.5%

## Methods
### Logistic Regression
Sequential experiments were conducted on:
- C
- Solver
- Class Weight

### Decision Tree
Sequential experiments were conducted on:
- Criterion
- CCP Alpha
- Min Samples Leaf
- Class Weight

### Ensemble Learning
- Hard Voting using the selected Logistic Regression and Decision Tree models

## Evaluation
Because the dataset is imbalanced, the F1-score of the minority class was used as the primary evaluation metric.

## Results
- Logistic Regression: F1-score = 51.09%
- Decision Tree: F1-score = 55.00%
- Hard Voting: F1-score = 52.53%

The tuned Decision Tree achieved the best performance among the three approaches.

## Tools
- Python
- pandas
- NumPy
- scikit-learn

## Key Learning
This project strengthened my understanding of:
- imbalanced classification
- hyperparameter experimentation
- model comparison
- regularization and pruning
- minority-class evaluation
