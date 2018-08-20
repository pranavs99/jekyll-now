---
layout: post
title: Sigmoid vs. softmax: What's the difference?
---

### What are they in the first place?

The sigmoid and the softmax function are both used in the same exact place: the output level of logistic regression. But how does it fit into the entire process?

If we have a classifier that sorts pictures into one of three classes: dog, cat, and goldfish, then the structure of the network will be the following: input layer, weight matrix, and then activation layer. The input layer is where we give our network each picture (probably as a flattened vector), which will influence a weight matrix via the loss function, and then output a continuous value. **Sigmoid and softmax functions are used here.**

##### The activation layer

You may have noticed that term when I was describing the neural network's structure: the *activation layer*. An activation layer is what separates a linear regression from a logistic regression, because a linear regression is simply a logistic regression without this layer.

The point of this activation layer is to turn the continuous values into class predictions. We can accomplish this by applying either the sigmoid or softmax **FINISH THIS 8/19 7:16pm**
