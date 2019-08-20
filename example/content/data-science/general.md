/*
Title: General questions
Description: Questions on Data Science
*/

**Model choice:**

My current model has a performance of 3.5% error rate and a new one has a performance of 3% error rate. Should I switch in production to the newer one?

Answer: Do statistical testing.

**What is hypothesis testing?**

Tests the validity of a claim (null hypothesis) that is made about a population using sample data. If the claim is not valid, then we accept
the alternative hypothesis as true.

[Article](https://towardsdatascience.com/p-values-explained-by-data-scientist-f40a746cfc8)

**What is a Z-score?**

Z-score is the number of standard deviations from the mean a data point is.

**What is a p-value?**

P-value is the probability that given a null hypothesis is true, it would be high enough so that we are not surprised by the evidence. If it is lower than a predefined significance layer (alpha) then we reject the null hypothesis and accept the alternative one.

[Article](https://towardsdatascience.com/p-values-explained-by-data-scientist-f40a746cfc8)

**What is the difference between one or two tailed tests?**

[Article](https://stats.idre.ucla.edu/other/mult-pkg/faq/general/faq-what-are-the-differences-between-one-tailed-and-two-tailed-tests/)

**What is precision?**

Used mostly in information retrieval (or binary classification), precision is a metric that defines how precise I am in my retrievals (or predictions). Meaning from the things I say they are class A (i.e. True), how many are they trully A? How precise am I in predicting A? More mathematically it is TP/(TP + FP).

**What is recall?**

Again used in informations retrieval, recall is a metric that defines how good my algorithm is in retrieving (or predicting) the correct documents (or classes) out of all the correct documents (or classes). It is the percentage of the documents denoted as A retrieved vs. all the A documents (retrieved or not). More methematically it is TP/(TP+FN)

**What is bayesian optimization?**

Bayesian optimization is a technique to optimise function that is expensive to evaluate.

[Article](https://www.kdnuggets.com/2019/07/xgboost-random-forest-bayesian-optimisation.html)

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

**What is Entropy?**

An indicator of how messy the data is

**What is the curse of dimensionality?**

Large space where the data reside which leads to sparse data that lead to random relations.

You can eliminate it by:

- Feature selection
- L1 regularization
- PCA, other dimensionality reduction techniques
- Better feature engineering

**Why ensembles are better?**

They make different errors.
