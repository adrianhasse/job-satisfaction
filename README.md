# JobSatisfaction
Predict job satisfaction using as input Stack Overflow’s annual Developer Survey of 2019

As data basis Stack Overflow’s annual Developer Survey of 2019 was taken to start with that analysis (https://insights.stackoverflow.com/survey/2019).

The notebooks try to predict job satisfaction and use Stack Overflow’s annual Developer Survey of 2019 as input. The random forest notebook, which is the main and best documented notebook, treats this ordinal regression as a normal regression problem. The gradient boosting notebook splits it in several problems to compute a probability distribution.

## Used libraries
I used pandas and numpy for data handling, scikit learn and light GBM for data processing and modelling and matplotlib, scipy and seaborn for data visualisation.

## Motivation of the project
The notebooks tries to answer 3 questions following the CRIS-DM process (https://www.sv-europe.com/crisp-dm-methodology/). The following explanation refers mainly to the notebook `developer_satisfaction_random_forest.ipynb`.

### Business Understanding
The following answers are the focus of this data analysis:
1. How satisfied are developers currently within their jobs?
2. What are the factors that influence job satisfaction the most?
3. Building on this, what should be considered to increase job satisfaction?

The first question is interesting to get an overview of the overall job satisfaction of developers and is purely descriptive. The second question needs a thourough analysis and modelling behind and is especially interesting for companies who want to keep their developers happy. The last question is more of a qualtitive nature and tackles possible actions to undertake improving satisfaction at a developer's working place.

### Data Understanding
Trying to answer these three questions, the `Stack Overflow’s annual Developer Survey` is a very good point to start since it also asks about job satisfaction. It is already a very clean dataset and well documented. The schema of the data is updated with explanation. To get a better data understanding please take a closer look in the notebooks and play around a little bit ;)

### Prepare Data
The data preparation is explained in detail in the notebook `developer_satisfaction_random_forest.ipynb`.

### Data Modeling
Data modeling is especially used to answer the second question. The notebook `developer_satisfaction_random_forest.ipynb` treats the underlying ordinal regression problem as a normal regression and uses therefore a random forest regressor. A more detailed explanation can be found inside the notebook.

### Evaluate the Results
This is especially referring to the third question is answered in detail in the following blog post linked below.

## Summary of the results
There exists a medium story which describes the thoughts and backround behind the analysis in more detail. Also, it gives a nice summary of the results. 
https://medium.com/@adrian.hasse/how-to-satisfy-developer-661843e3c9a7?source=friends_link&sk=8685e33ec2134661d7bfd2d1aa96a89f

