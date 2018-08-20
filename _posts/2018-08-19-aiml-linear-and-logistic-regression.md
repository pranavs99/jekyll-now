---
layout: post
title: Linear and logistic regression
---

In this post, we're going to look at the absolute backbone of machine learning: regression. We'll start off with explaining both linear and logistic regression separately, and then we'll compare and contrast them.

## What is regression?

Before we even talk about regression, we need to talk about the goal of statistics: to determine knowledge from data points. Regression is simply a manifestation of that. In *simple linear regression*, which is where we'll start, we're going to try to come up with an equation of a line that best represents the data we have here. This is known as the *line of best fit*.

*An important aside: regression is not used when there is a deterministic relationship, such as diameter to circumference. Regression is only used when there is no known deterministic relationship and we must therefore attempt to establish a* statistical relationship.

![_config.yml]({{ site.baseurl }}/images/regression3.png)

In this graph, we have a set of data points relating height and weight. Height is graphed along the *x*-axis, while weight is graphed along the *y*-axis. This tells us that weight is **dependent** on height. In fact, we can establish some terminology for the axes: the horizontal axis is the *predictor variable* and the vertical axis is the *response variable*, or the variable whose value we're trying to predict. Now, let's come up with the *line of best fit*. Here's the general equation:

![_config.yml]({{ site.baseurl }}/images/equationofaline.gif)

The *y* term represents the *response variable* and the *x* term represents the *predictor variable*. What about the *m* and the *b*? They're what give the *line of best fit* its best-fitting properties. The *m* term is commonly referred to as slope. It's the amount that the *response variable* increases for every change of **1 unit** in the *predictor variable*, and it's incredibly important because it shows how much the *predictor variable* influences the *response variable*. For example, an *m*-value of 50 in our height-weight example would mean that for every change of 1 inch in the height, the weight would change by 50 pounds. But what direction would the change go?

It depends on the direction of the relationship. A *positive relationship* is a relationship where an **increase** in the *predictor variable* leads to an **increase** in the 
