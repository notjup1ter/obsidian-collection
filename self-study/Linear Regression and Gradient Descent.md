---
class:
date: 2026-02-21
---
# Resources
---
https://www.youtube.com/watch?v=4b4MUYve_U8&list=PLoROMvodv4rMiGQp3WXShtMGgzqpfVfbU&index=2



In general, we can generate a predicted value for a dependent variable based on a given set of parameters $x_{1}, x_{2}, \dots x_{n}$, where $n$ is the number of features. For these features, each has a corresponding weight or [[parameter]] ($\theta$). With this form, we can make a [[Multiple Linear Regression Model]] as follows:
$$y = \theta_{1}x_{1} + \theta_{2}x_{2} + \dots + \theta{n}x_{x}$$
where y is the response variable we are interested in (typically quantitative for MLR, example: height in inches), and each $\theta$ is each features's weight/parameter.

Typically speaking, we do not know, immediately, what the parameters have to be in order to optimize prediction. As a result, we need a way to find said parameter value that minimizes the [[residual error]] / [[cost]] 