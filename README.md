## Machine-Learning


### Pre-processing and Visualization
1. Missing data
  - Omission
    - remove rows >> .dropna(axis=0)
    - remove columns >> .dropna(axis =1)
  - Imputation
    - fill with zero >> SimpleImputer(strategy = 'constant', fill_value = 0)
    - fill with mean >> SimpleImputer(strategy = 'mean')
    - fill with median >> SimpleImputer(strategy = 'median')
    - fill with mode >> SimpleImputer(strategy = 'most_frequent')
3. Outliers
4. Normalization

### Supervised Learning
Feature selection, Regularization, Feature engineering

### Unsupervised Learning
Cluster algorithm selection, Feature extraction, Dimension reduction

### Model Selection and Evaluation
Model generalization and evaluation, Model selection
