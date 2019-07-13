## Random Forests

### Describe how random forest works, pros and cons, and where have you used them lately?

It is an ensemble method that creates many decision trees by selecting randomly different combinations of attributes in order to build the trees, making it more difficult to overfit. In the end the tree are aggregated. Params to usually tune are:
  - number of trees, and
  - number of features to be selected at each node;

Pros:
 - Works on a lot of datasets (Fernadez-Delgado et al., JMLR, 2014)
 - Few important parameters to tune
 - Handles multiclass problems (unlike SVMs)
 - Can handle a mixture of features and scales
 
Cons:
 - Slow for real-time prediction due to the large number of trees.
 - When there are categorical values with different number of levels, RF prefer the variables with more levels.
 
 
### Describe how XGBoost works, pros and cons

It is an ensemble method that follows the boosting approach. It builds trees one at a time, with each tree correcting the errors made by the previous one. Params to usually tune are:
  - number of trees, 
  - depth of trees, and 
  - learning rate.

Pros:
- Helpful in highly imbalanced class problems (outlier detection)
- Kagglers are drinking in its name :)

cons:
- Sensitive to overfitting if data is noisy
- Long(er) training times due to the sequential nature
- Harder to tune
- More of a black-box even though tree-based

## Links

- [1](https://www.kdnuggets.com/2019/07/xgboost-random-forest-bayesian-optimisation.html)
