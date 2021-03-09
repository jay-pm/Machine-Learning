## Machine-Learning


### Pre-processing and Visualization
**1. Missing data**  
Why bother about missing data?  
  - how you handle missing values can introduce bias, so handling it appropriately will reduce that probability.
  - Most ML algorithms require complete data (else an error is generated)  
Note: the best approach is to try out all below techniques for filling missing value and adopt the one which has **least impact on variance of dataset**.

  - Omission (removing rows or columns can remove too much of data)
    - remove rows >> .dropna(axis=0)
    - remove columns >> .dropna(axis =1)
  - Imputation
    - fill with zero >> SimpleImputer(strategy = 'constant', fill_value = 0) *[Bias results downwards]*
    - fill with mean >> SimpleImputer(strategy = 'mean') *[affected more by outliers]*
    - fill with median >> SimpleImputer(strategy = 'median') *[better in case of outliers]*
    - fill with mode >> SimpleImputer(strategy = 'most_frequent') *[have varying degree of helpfullness]*
    
3. Outliers
4. Normalization

### Supervised Learning
**1. Feature selection**  
Selecting correct features is important because it:
1. reduces overfitting
2. improves accuracy
3. increases interpretability.


, Regularization, Feature engineering

### Unsupervised Learning
Cluster algorithm selection, Feature extraction, Dimension reduction

### Model Selection and Evaluation
Model generalization and evaluation, Model selection
