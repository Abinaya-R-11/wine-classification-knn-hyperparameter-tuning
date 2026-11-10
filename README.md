 # Wine Classification using K-Nearest Neighbors (KNN)

This project applies the K-Nearest Neighbors (KNN) algorithm to classify wines into three cultivator classes based on chemical characteristics.

## What is in this project?
- Dataset: Scikit-Learn's built-in Wine recognition dataset (178 samples, 13 chemical features, 3 target classes).
- Feature Scaling: Applied StandardScaler so that all chemical measurements contribute equally to distance calculations.
- Baseline Evaluations: Evaluated model performance across baseline neighbor counts ($K = 3, 5, 7, 9$).
- Hyperparameter Tuning: 
  - Implemented 5-Fold Cross-Validation (KFold(n_splits=5)) across candidate values from $K = 3$ to $51$.
  - Visualized mean cross-validation accuracy versus neighbor count using matplotlib.
- Optimal Model: Identified $K = 21$ as the optimal neighbor parameter, achieving an accuracy of ~97.2% on training data and ~97.7% mean CV score.
## Key Takeaway
Because KNN relies on geometric distance metrics (such as Euclidean distance), standardizing features is essential to prevent larger-scale features (like Proline or Magnesium) from dominating the neighbor search.

## Tools Used
- Python
- Pandas
- Scikit-Learn
- Matplotlib
