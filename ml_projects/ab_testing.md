# AB testing also known as split testing
> “A/B testing is a way to compare two versions of something to figure out which performs better.”

running an AB test:

- Feature flagging and randomization: how you determine who sees what variant (e.g., which experience or features)
- Metrics: what we measure to determine which variant wins and that we don’t inadvertently break anything in the process
- Statistics: the fancy math way of determining whether or not a metric for a given variant is better than another variant
- Drawing conclusions: how we make decisions from the metrics and statistics

# Statistical Steps to approach AB Testing
### AB Testing method tests the  - significance of difference in a metric variable values - between 2 groups 

## Step 1: Normality Assumption

Goal: if the series have normal distribution or not 
  * Box PLot -- see outliers
  
Choose between Independent Samples t Test and Mann-Whitney U Test
- If p value of the test is > .05 => Independent samples T Test.
- If p value of the test is < .05 => Mann-Whitney U Test.

## Step T-test -- Testing the Homogeneity Assumption

Goal: choose which code setting to perform t-test

- If p value of the test is > .05 Independent Samples t Test = `equal_var=True` extention.
- If p value of the test is < .05 Independent Samples t Test = `equal_var=False` extention. -> which indicates that H0 is rejected.

## Statistics
T-test -- a significant difference between the **means** of two groups of data.
U-Test --- a significant difference between the **distributions** of two groups of data.
