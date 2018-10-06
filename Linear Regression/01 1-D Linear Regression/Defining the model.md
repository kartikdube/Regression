# Simple Linear Regression

Or line of best fit is defined as ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/bf2c1cac7c1e6c9a426d92e9adad6ff4d8b4152e), where which describes a line with slope β and y-intercept α.

In general such a relationship may not hold exactly for the largely unobserved population of values of the independent and dependent variables; we call the unobserved deviations from the above equation the errors. 

Suppose we observe n data pairs and call them {(xi, yi), i = 1, ..., n}. We can describe the underlying relationship between yi and xi involving this error term εi by 

![](https://wikimedia.org/api/rest_v1/media/math/render/svg/968be557dd22b1a2e536b8d22369cfdb37f58703)

This relationship between the true (but unobserved) underlying parameters α and β and the data points is called a linear regression model. 

The goal is to find estimated values 
![](http://latex.codecogs.com/png.latex?%5Chat%7B%5Calpha%20%7D) and 
![](http://latex.codecogs.com/png.latex?%5Chat%7B%5Cbeta%20%7D)
for the parameters α and β which would provide the "best" fit in some sense for the data points.
In this article the "best" fit will be understood as in the least-squares approach: a line that minimizes the sum of squared residuals 
![](http://latex.codecogs.com/png.latex?%5Chat%7B%5Cvarepsilon%20%7D_%7Bi%7D) 
(differences between actual and predicted values of the dependent variable y), 
each of which is given by, for any candidate parameter values a and b.

![](https://wikimedia.org/api/rest_v1/media/math/render/svg/fa95dc245447e9c8fffc5dd621b03223816b0f4f)

In other words,

![](https://wikimedia.org/api/rest_v1/media/math/render/svg/d78d9728a09420ccf040643bec19b79d6aa8a748)

By expanding to get a quadratic expression in a and b , we can derive values of a  and  b that minimize the 
objective function Q (these minimizing values are denoted 
![](http://latex.codecogs.com/png.latex?%5Chat%7B%5Calpha%20%7D) and 
![](http://latex.codecogs.com/png.latex?%5Chat%7B%5Cbeta%20%7D) )

![](https://wikimedia.org/api/rest_v1/media/math/render/svg/ac3b42d4d7b7d8d496bbca97266021f73cceac84)

where,

![](http://latex.codecogs.com/png.latex?%5Cbar%7Bx%7D)  and ![](http://latex.codecogs.com/png.latex?%5Cbar%7By%7D)as the average of the xi and yi, respectively

rxy as the sample correlation coefficient between x and y

sx and sy as the uncorrected sample standard deviations of x and y

Var and Cov as the sample variance and sample covariance, respectively

Substituting the above expressions for 
![](http://latex.codecogs.com/png.latex?%5Chat%7B%5Calpha%20%7D) and 
![](http://latex.codecogs.com/png.latex?%5Chat%7B%5Cbeta%20%7D) into 

![](https://wikimedia.org/api/rest_v1/media/math/render/svg/338685159bfacab3efd907db4fcd8611381c0098)

![](https://wikimedia.org/api/rest_v1/media/math/render/svg/349bd74b3ca0b298b1314c8364ec91a0a1b0499e)

This shows that rxy is the slope of the regression line of the standardized data points (and that this line passes through the origin).
Generalizing the ![](http://latex.codecogs.com/png.latex?%5Cbar%7Bx%7D) notation, 
we can write a horizontal bar over an expression to indicate the average value of that expression over the set of samples. 

![](https://wikimedia.org/api/rest_v1/media/math/render/svg/3d570a1ea8bb90927e92f82d3864e4ade0447024)

![](https://wikimedia.org/api/rest_v1/media/math/render/svg/1f21324fcf481023ee5fafea8f4846f602c9c8f9)

The coefficient of determination ("R squared") is equal to ![](http://latex.codecogs.com/png.latex?r%5E%7B2%7D_%7Bxy%7D) when the model is linear with a single independent variable. See sample correlation coefficient for additional details. 

