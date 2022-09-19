# Machine learning model and its implementations

### Convention and Notations
Dependent variable = output variable <br>
Independent variable = input variable<br>
actualValue = actual datapoint region<br>
predictedValue = predicted datapoint region<br>

## Linear Regression
1. Linear regression is the very first algorithm to study before any other algorithms. Speaking from the experience. <br>
2. It is <b>supervised learning algorithm</b> which solves <b>regression problem</b>.<br>
3. Common computation happens with the equation of straight line - y = mx + c <br>
4. It has 3 types of analysis - Simple or univariate linear regression, <b> Multiple or multi-variate Linear regression</b> and polynomial regression.

### Simple Linear Regression (Uni-variate)
Where only one dependent variable is present and the model has to find the linear relationship with independent variable. <br>
{0,1,2,3,...., n-1} fit in the line - <b>predictedValue</b> = mx + c <br>
Where the model has to find or learn m and c to find the best fit line for x variable. <br>
<b>Error function</b> = (actualValue - predictedValue)^2 <br>

### Multiple Linear Regression (Multi-variate)
Where there are more than one independent variable for the model which has to find the relationship with dependent variables. <br>
{m0, m1x1, m2x2, m3x3,....,mnxn} fits the line - <b>predictedValue</b> = Transpose(m)*x + c <br>

### Polynomial Regression
Polynomial regression exist to provide justification to the fitting capability of the linear regression which used to assume the relationshop between the point is linear in nature. <br>
{m0, m1x, m2x^2, m3x3,...., mnx^n} fit in with the line that shows the relationshop with introducing a polynomial degree.

### Error Functions
#### Sum of Square Total (SST)
- Measures the total variability of the dataset. <br>
- Sum (actualValue - mean(actualValue))^2 <br>

#### Sum of Square Regression (SSR)
- Measures the explained variability by the line. <br>
- Sum (predictedValue - mean(actualValue))^2

#### Sum of Square Error (SSE)
- Measures the unexplained variability by the regression. <br>
- sum (actualValue-predictedValue)^2

### Error/Loss/Cost Function
#### Mean Absolute Error
- Calculation of absolute resudual value of all data points. <br>
- MAE = (1/N) * sum(|actualValue - predictedValue|).<br>
- Doesnt indicate the under and over performance of the model. <br>

#### Mean Square Error
- Square the difference between the sum of all data points. <br>
- MSE = (1/N) * sum(actualValue - predictedValue)^2 <br>
<i> Ps. N = total number of datapoints</i>
<i> Choice between MSE and MAE depends on how anyone wants to treat large errors. </i>

## Outliers
- Outlier is the datapoint which is far from the expected reason or simply data point which shows sudden spikes in the dataset. <br>
- We use the outliers only when it has some meaning or depending on the field of study.

## Task now becomes Finding the value of slope(m) and intercept (c)
We can gain the value of slope and intercept by using different approaches. 
1. For univariate <br> 
We Can use <b>OLS (Ordinary Least Squares)</b> <br>
m = sum(actualValue- mean(actualValue))/sum((actualValue - mean (actualValue))^2)

### Gradient Decent
It is an iterative optimization algorithm to find the minimum of the function. (minimum = less error)<br>
Steps to compute gradient descent,<br>
1. We calculate the partial derivate of RMSE against m and c.
2. then we update m and c respective to multiplcation of a small learning rate.<br>
3. Formula, m = m - L * deriation(m) and c = c - L * derivation(c) <br>
4. Repeat the process until we find an optimal value of m and c.<br>

### Evaluation Merics
We can evaluate linear regression using, R squared or RMSE.<br>
1. R squared or coefficient of determination.<br>
- Ratio of variation / total variation<br>
- The value of Rsquared should be between 0 to 1 and value more closer to 1 the better. <br>
- r = 1 - SSR/SST<br>

2. RMSE
- It is difference of actual and predicted values.
- RMSE = sqrt ((1/n)* sum(actualValue - predictedValue)^2)

## Use cases.
Some common example of problem that is solved using linear regression is,<br>
Predicting the price of house based on features. <br>
Predicting the sales based on input parameters. <br>
Forecasting sales.<br>
Predicting weather and many more.
