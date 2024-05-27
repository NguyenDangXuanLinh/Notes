# Symbol
Square -- bình phương (* chính nó 2 lần) luỹ thừ 2
root -- căn
Square root -- căn bậc 2
coefficient -- hệ số
variation -- biến động 
power -- number of times that an amount is to be multiplied by itself

# Linear Regression
Residual -- difference between actual & prediction |y - yhat|

## Models Comparision
### Compare errors of each model
Cost function (total loss) = loss (single train point) = error -- 2 functions:
    - MSE = sum(y -yhat)^2 / total n
    - RMSE = root(mse)
    
### Just because model is the best, doesn't mean model is GOOD
Create a scale 0 to 1 : very bad model - to - very good model -- use that to compare
--> R^2 -- coefficient(para) of determination
    ``` R^2 = 1 - sum(yhat - y) / sum(y.avg - y)

# Linear Regression Coefficient (Parameter)
Example: we have model of y = 1.01x + 103, where y is the sales in 1,000 units and x is the advertising budget in $1,000 for TV, radio, newspaper
- The sales coefficient in the regression equation is 1.01. This coeffiecient represents the mean increase of sales for every dollar additional in TV budget

 ```
- Interpretation: for every dollar invested in advertising gets me $1.01 back in sales, which is 1% net increase
-> Important question: how certain are we in our estimation of the coefficient 1.01
```


  
## How reliable are the model interpretation?
**If we have multiple predcitors: EX predict sales using ads, newspaper, tv..**
1. Which predictors are most important?
2. Which of them really affect the out comes?
   ( I am the best swimmer in my family, does not mean I qualify to join Olympic)

 Ex: my model for advertising: y = 1.01x + 120, where y is the sales in $1,000 units and is the TV budget  
## Hypothesis Testing and Significance   
How do we assess if there is a true relationship between outcome & predictors?
Problem: multiple predictors -> how to know which one affect 
