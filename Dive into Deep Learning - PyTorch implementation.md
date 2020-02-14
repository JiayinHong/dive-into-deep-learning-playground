### Dive into Deep Learning - PyTorch implementation

------

#### 1. Linear Neural Networks

##### 1.1 Linear Regression

Take the following linear model as an example.
$$
price=w_{area}\cdot area+w_{age}\cdot age+b\tag{1.1.1}
$$
Here, $w_{area}$ and $w_{age}$ are called *weights*, and *b* is called a *bias* (also called an *offset* or *intercept*).

The weights determine the influence of each feature on our prediction, and the bias just says what value the predicted price should take when all of the features take value 0.

When our inputs consist of *d* features, we express our prediction $\hat{y}$ as
$$
\hat{y}=w_1\cdot x_1+...+w_d\cdot x_d+b\tag{1.1.2}
$$
Collecting all features into a vector $\mathbf{x}$ and all weights into a vector $\mathbf{w}$, we can express our model compactly using a dot product:
$$
\hat{y}=\mathbf{w}^{T}\mathbf{x}+b\tag{1.1.3}
$$
