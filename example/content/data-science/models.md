/*
Title: Models
Description: Different machine learning models
*/

## Decision Trees

**How is a decision tree built?**
(Common question)

**How do I prune a decision tree?**

**What happens if I choose randomly the split?**

## Support Vector Machines

**Which kernel to choose?**

**What data do I need for each kernel?**

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

## LSTM

Tutorials:
- [Understanding LSTM](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)

- Cell state: the cell state runs through the LSTM with minor interations
- Forget gate layer: Decides what information will be thrown away from the cell state through a sigmoid layer (1 keep this, 0 get rid of this)
- Input gate layer: Decides what new information will go into the cell state
- Output gate layer: Decides what cell state information will be outputed

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
