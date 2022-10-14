# Logistic Regression

Logistic regression is a statistical analysis to predict a binary outcome, such as True or False, Yes or No based on prior observations of a dataset. <br>

Logistic Regression predicts a dependent variable by analyzing the relationship between one or more existing independent variables. <br>

Eg. This model can be ised to predict political candidate will win or lose on election, a high school student will be able to admitted or not to a particular college, can experiment on Titanic dataset either a passenger will survive the disaster or not. Basically a straight foreward answer to YES OR NO. A logistic regression model can take into consideration multiple input criteria. In the case of college acceptance, the logistic function could consider factors such as the student's grade point average, SAT score and number of extracurricular activities. Based on historical data about earlier outcomes involving the same input criteria, it then scores new cases on their probability of falling into one of two outcome categories.<br>

<b> PS. Logistic regression can also play a role in data preparation by allowing data set to be put int specifically predefined bucket during <i> Extract, Transform and Load (ETL) </i> </b>

### Logistic Regression Equation
The logistic regression equation can be obtained from the Linear Regression equation. So we have, <br>

y = b0 + b1x1 + b2x2 + ... + bnxn <br>


In logistic regression y can be between 0 and 1 so for this lets divide the equation by (1-y): <br>

y/(1-y) such that 0 for y = 0 and infinity for y=1 <br>

But we need range between negative infinity to positive infinity then we take <b>LOG</b> for the equation: <br>

log(1/(1-y)) = b0 + b1x1 + b2x2 + b3x3+ ... bnxn <br>

### Types of logistic regression

On the basis of categories it can be divided into three types: <br>

1. Binomial: there can be only two possible types of the dependent variable.<br>
2. Multinomial: there can be 3 or more possible unordered types of dependent variable eg. cat, sheep, dog <br>
3. Ordinal: there can be 3 or more pssible ordered types of depentent variables, such as low, medium, high. <br>


### Business achievement using logistic regression

Organization uses insight produced by logistic regression to enhance their business strategy for achieving business goals such as reducing expenses or losses and increasing the ROI in marketing campaigns. <br>
Likewise, a credit card company will develop a model to help it predict if a customer is going to default on its credit card based on such characteristics as annual income, monthly credit card payments and the number of defaults. In banking parlance, this is known as default propensity modeling.<br>