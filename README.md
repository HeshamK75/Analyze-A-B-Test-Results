# Analyze A/B Test Results
A/B tests are very commonly performed by data analysts and data scientists.  It is important that you get some practice working with the difficulties of these   For this project, you will be working to understand the results of an A/B test run by an e-commerce website.  Your goal is to work through this notebook to help the company understand if they should implement the new page, keep the old page, or perhaps run the experiment longer to make their decision.

This project consist of 3 parts as below


## Probability based approach:

 probability of an individual receiving the new page is 0.5001
 so there is almost the same chance that an individual received the old page
 
 ## A/B test:
* In A/B test we set up our hypothesis to test if new page results in better conversion or not
* We simulated our user groups with respect to conversions
* We found the P-Value = 0.1899
* With such a p-value, we didnt reject null hypothesis
* By using the built-in stats.proportions_ztest we computed z-score and p-value which confirmed our earlier p-value and failure to reject null hypothesis

## Regression

* We looked at exploring two possible outcomes. Whether new page is better or not.
* With logistic regression results, we again encountered same z-score as well as p-value of 0.190, corresponding two-tailed case
* By further adding geographic location of the users, we tried to find if any specific country had an impact on conversion
* The result gave a similar outlook and suggested that the countries have no impact on the conversion rate.


### Used Tools
Jupyter notebook
Python and it's libraries (pandas, numpy, matplotlib)
