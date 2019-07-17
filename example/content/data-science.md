/*
Title: Data Science
Description: Questions on Data Science, Machine Learning, Deep Learning etc.
*/

**What is precision?**

Used mostly in information retrieval (or binary classification), precision is a metric that defines how precise I am in my retrievals (or predictions). Meaning from the things I say they are class A (i.e. True), how many are they trully A? How precise am I in predicting A? More mathematically it is TP/(TP + FP).

**What is recall?**

Again used in informations retrieval, recall is a metric that defines how good my algorithm is in retrieving (or predicting) the correct documents (or classes) out of all the correct documents (or classes). It is the percentage of the documents denoted as A retrieved vs. all the A documents (retrieved or not). More methematically it is TP/(TP+FN)

**What is bayesian optimization?**

Bayesian optimization is a technique to optimise function that is expensive to evaluate.

**What does the p-value mean?**

TODO.

**Boundaries: Provide the decision boundaries of different algorithms**

- Naive Bayes
- Logistic Regression
- Decision Trees

**What is a ROC curve?**
GUI representation of TPR vs. FPR

**What is a Type I error?**
False Positive Rate

**What is a Type II error?**
False Negative Rate

**Bayes Theorem**
Posterior probability of an event given what is know as prior knowledge.

`P(A|B) = P(B|A) * P(A) / P(B)`

i.e.

`P(Spam|Words) = P(Words|Spam) * P(Spam) / P(Words)`

**Bagging**
Different models built on different subsets of data

**Boosting**
Different weights to each sample

## Regularization techniques

**L1**
Lasso, minimize absolute value

**L2**
Ridge, minimize square value

**Dropout**
Set randomly outputs to 0 (disables them). This prevent neurons from co-adapting and forces them to learn individually useful features. 

**Early Stopping**

## Bias-Variance trade-off

- Bias: Error due to erroneous or overly simplistic assumptions, underfitting.
- Variance: Too much complexity, sensitive to high degrees of variation, overfitting.

**How can I act if I have different kinds of high/low bias/variance scenarios**

## Random Forests

**Describe how random forest works, pros and cons, and where have you used them lately?**

Based on Bagging. It is an ensemble method that creates many decision trees by selecting randomly different combinations of attributes in order to build the trees, making it more difficult to overfit. In the end the tree are aggregated. Params to usually tune are:
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
 
 ## Boosting Machines

**Describe how XGBoost works, pros and cons**

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

## Convolutional Neural Networks

A convolution is the process of applying a filter (“kernel”) to an image. Max pooling is the process of reducing the size of the image through downsampling.

- CNNs: Convolutional neural network. That is, a network which has at least one convolutional layer. A typical CNN also includes other types of layers, such as pooling layers and dense layers.
- Convolution: The process of applying a kernel (filter) to an image
- Kernel / filter: A matrix which is smaller than the input, used to transform the input into chunks
- Padding: Adding pixels of some value, usually 0, around the input image
- Pooling The process of reducing the size of an image through downsampling. There are several types of pooling layers. For example, average pooling converts many values into a single value by taking the average. However, maxpooling is the most common. Usefull for decreasing computational power required and ectracting dominant features which are rotational and positional invariant.
- Maxpooling: A pooling process in which many values are converted into a single value by taking the maximum value from among them. Performs as a noise suppressant as well.
- Stride: the number of pixels to slide the kernel (filter) across the image.
- Downsampling: The act of reducing the size of an image

**Why use CNNs?**
To build invariance in your model. When recognizing an object in one place, CNNs will recognize it to others as well. A CNN succesfully captures Spatial and Temporal dependencies in an image.

**Links**

- [A Comprehensive Guide to Convolutional Neural Networks — the ELI5 way](https://towardsdatascience.com/a-comprehensive-guide-to-convolutional-neural-networks-the-eli5-way-3bd2b1164a53)

## Links

- [1](https://www.kdnuggets.com/2019/07/xgboost-random-forest-bayesian-optimisation.html)