- For in-dept knowledge:
andrew-ng-machine-learning-yearning

# Things to consider to ensure a good results from ML
## Data sets
Problems for poor performance is -- the training distribution is different from the distribution I ultimately care about
=> the most important changes to make to the machine learning system.

We usually define:
  - Training set —  run your learning algorithm on.
  - Dev (development) set — use to tune parameters, select features, and make other decisions regarding the learning algorithm. Sometimes also called the **hold-out cross validation set**.
  - Test set —  evaluate the performance of the algorithm, but **not to make any**__ decisions regarding what learning algorithm or parameters to use

### Best preactice --- Try to pick test examples that reflect what you ultimately want to perform well on

## Same and Different Distributions Problems on dev and test sets
### Same -- overfit dev set -> more data
### Different -- 2 potential:
- overfit dev set
- test set is harder than dev  -> algorithm might do well but no significant improvement
- test is not harder, but sifferent from dev -- example: predict car sales in 4 countries, divides 2 contries each to dev and test set
  => ### If purpose is ml application results -> same distribution
  => ### if focusing on research algorithm progress -> diff distribution

## How large a dwv set?
Goal: dev set is large enough to detect differences between algorithms 
> Dev sets with sizes from 1,000 to 10,000 examples are common. Because with 10,000 examples, I might able to detect an improvement of 0.1%
## Direct impact on the company’s profits for mature and important applications even a 0.01% improvement needs much larger than 10,000,—for example, advertising, web search, and product recommendations.

## Bias and Variance
The bias -- the trainning error (check algorithm)
The variance -- how much worse I do on test set, compared with training set (check generalization)
    Total error = bias + variance (in MAE error)
