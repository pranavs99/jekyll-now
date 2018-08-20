---
layout: post
title: Linear and logistic regression
---

In this post, we're going to look at the absolute backbone of machine learning: regression. We'll start off with explaining both linear and logistic regression separately, and then we'll compare and contrast them.

## What is regression in the first place?

Before we even talk about regression, we need to talk about the goal of statistics: to determine knowledge from data points. Regression is simply a manifestation of that. In **simple linear regression**, the act of regression on a two-variable graph, we're going to come up with an equation of a *line* that best represents the data we have here. This is known as the **line of best fit**.

*An important aside: regression is not used when there is a deterministic relationship, such as diameter to circumference. Regression is only used when there is* no known deterministic relationship *and we must therefore attempt to establish a* statistical relationship.

![_config.yml]({{ site.baseurl }}/images/regression3.png)
*taken from* https://support.minitab.com/en-us/minitab-express/1/help-and-how-to/graphs/scatterplot/create-the-graph/choose-a-scatterplot/

In this graph, we have a set of data points relating height and weight. Height is graphed along the *x*-axis, while weight is graphed along the *y*-axis. This tells us that weight is *dependent* on height. In fact, we can establish some terminology for the axes: the horizontal axis is the **predictor variable** and the vertical axis is the **response variable**, or the variable whose value we're trying to predict. Now, let's come up with the line of best fit. Here's the general equation:

![_config.yml]({{ site.baseurl }}/images/equationofaline.gif)

The *y* term represents the response variable and the *x* term represents the predictor variable. What about the *m* and the *b*? They're what give the line of best fit its best-fitting properties. The *m* term is commonly referred to as slope. It's the amount that the response variable increases for every change of ***1 unit*** in the predictor variable, and it's incredibly important because it shows how much the predictor variable influences the response variable. For example, an *m*-value of 50 in our height-weight example would mean that for every change of *1 inch* in the height, the weight would change by *50 pounds*, while an *m*-value of 0.2 would mean that for every change of *1 inch* in the height, the weight would change by *0.2 pounds*. But what direction would the change go? It depends on the direction of the relationship. 

A *positive relationship* is a relationship where an **increase** in the predictor variable **leads to an increase** in the response variable and a **decrease** in the predictor variable **leads to a decrease** in the response variable. An example of this would be the height-weight example that we have. We can do a little check to see if a scatter plot follows a positive relationship: if we move our finger to the right and the points start to get higher, while moving our finger to the left will cause the points to get lower, we're home free. A *negative relationship* is a relationship where an **increase** in the predictor variable **leads to a decrease** in the response variable and a **decrease** in the predictor variable **leads to an increase** in the response variable. An example of this is shown below. If we move our finger to the left, we should see the points getting higher, while moving our finger to the right should show the points getting lower.

These relationships are made mathematical by the *sign* of the *m*-value. A positive relationship is signified by an _m_-value greater than 0 (or just positive), while a negative relationship is signified by an _m_-value less than 0 (or just negative).

But then we arrive at the *b* term because of the situations where *x* = 0. If there wasn't a constant added to the entire equation, every single graph would have a (0, 0) point. That just doesn't make sense. For the height-weight example, you could say that it might, but when you look at an age-height example, (0, 0) doesn't make any sense. We aren't born at age 0 with a height of 0 inches! Instead, we have to "offset" the line by a certain term to make sure that the *x* = 0 case makes sense. Formally, the *b* term is known as the __y-intercept__.


