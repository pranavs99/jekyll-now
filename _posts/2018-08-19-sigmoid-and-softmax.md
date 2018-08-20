---
layout: post
title: Sigmoid and softmax: What are they and what's the difference?
---

In this post, we're going to learn what the sigmoid and softmax functions are, where they're used, why they're used there, and compare them so you know which one to use.

## What are they in the first place?

The sigmoid and the softmax function are both used in the same exact place: the output level of logistic regression. But how does it fit into the entire process?

If we have a classifier that sorts pictures into one of three classes: dog, cat, and goldfish, then the structure of the network will be the following: an input layer, a weight matrix, and then an activation layer. The input layer is where we give our network each picture (probably as a flattened vector), which will influence a weight matrix via the loss function, and then output a continuous value.

### What's the activation layer?

This is where the sigmoid and softmax function come in. An activation layer is what separates a linear regression from a logistic regression: it transforms what are previously continuous values into *class predictions*. 

**FINISH THIS 8/19 7:16pm**
