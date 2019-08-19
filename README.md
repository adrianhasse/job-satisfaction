# JobSatisfaction
Predict job satisfaction using as input Stack Overflow’s annual Developer Survey of 2019

As data basis Stack Overflow’s annual Developer Survey of 2019 was taken to start with that analysis (https://insights.stackoverflow.com/survey/2019).

Both notebooks try to predict job satisfaction and use Stack Overflow’s annual Developer Survey of 2019 as input. The random forest notebook treats this ordinal regression as a normal regression problem. The gradient boosting notebook splits it in several problems to compute a probability distribution.

## Used libraries
I used pandas and numpy for data handling, scikit learn and light GBM for data processing and modelling and matplotlib, scipy and seaborn for data visualisation.

## Motivation of the project
This notebook tries to answer the following questions:

1. How satisfied are developers currently within their jobs?
2. What are the factors that influence job satisfaction the most?
3. Building on this, what should be considered to increase job satisfaction?

## Summary of the results
There exists a medium story which describes the thoughts and backround behind the analysis in more detail. Also, it gives a nice summary of the results. 
https://medium.com/@adrian.hasse/how-to-satisfy-developer-661843e3c9a7?source=friends_link&sk=8685e33ec2134661d7bfd2d1aa96a89f

