/*
Title: Biad-Variance trade-off
Description: Questions on bias variance trade-off
*/

**Definitions**

- Bias: Error due to erroneous or overly simplistic assumptions, underfitting. The error rate on the training set.
- Variance: Too much complexity, sensitive to high degrees of variation, overfitting. The error rate between the training and the validation set.

**How can I act if I have different kinds of high/low bias/variance scenarios**

High Bias:
- Increase model size (usually with regularization to mitigate high variance)
- Add more helpful features (which is another way of increasing again model size)
- Remove (Worse) / reduce (Better) regulaization
- Adding more training data wont help...the model is too "small"

High variance:
- Add training data (usually with a big model to handle them)
- Add/increase regularization
- Early stopping for NN
- Remove features (make the model simpler)
- Decrease model size (prefer regularization)
- Add more helpful features that are more useful to the problem at hand instead of the ones you have

**Can I have both low variance-low bias or high bias-high variance?**