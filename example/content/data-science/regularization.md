/*
Title: Regularization
Description: Questions on regularization
*/

**L1**

Lasso, minimize absolute value

**L2**

Ridge, minimize square value

**Dropout**

Set randomly outputs to 0 (disables them). This prevent neurons from co-adapting and forces them to learn individually useful features. 

**Early Stopping**

**How do you select hyperparameters?**

1. Manual Search
2. Grid Search
3. Random Search
4. Bayesian Optimization

Check this as well: [Guideline to select the hyperparameters in Deep Learning](https://stats.stackexchange.com/q/95495/57185)

**What is batch normalization?**

It is the normalisation the inputs of each layer in such a way that they have a mean output activation of zero and standard deviation of one.

The idea is to do the same in the hidden layers as you do in the input layer.

Batch normalization:

- Makes the network learn faster (converge more quickly, higher learning rates)
- Helps with weight problems (weight initialization, saturated activation functions, some regularization capabilities)