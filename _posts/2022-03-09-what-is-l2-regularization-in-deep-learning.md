---
title: "What is L2 Regularization in Deep Learning?"
mathjax: true
layout: post
---

One of the major problems encountered in the field of Machine Learning is overfitting, or the inability of our model to make accurate predictions on general datasets. A model which is overfitted usually performs very well in the dataset it was trained on. However, when used on to predict on another dataset, the model performs poorly. Such a model is also said to have high variance. Regularization is a technique in Deep Learning that is used to reduce the variance or prevent overfitting of our network. 



![l2](/assets/l2.png)

There are different types of Regularization techniques that can be implemented. However before discussing regularization, let us look at the cost function of a logistic regression or neural network model without any regularization, which is given by:

$$ J(w,b)=frac{1}{m}sum{i=1}^m L(\hat{y^i},y^i) $$

Here, L could be any loss function that we use depending on our predictive task (classification or regression) , $$ m $$ denotes the total number of records and $$ w \in [R^{n_x}] $$,$$ b\in[ʀ] $$ denotes our parameter of weights and biases respectively. Here, $$ n_x $$ denotes the number of input features. Now that we have that as reference, let us dive into L2 Regularization.

