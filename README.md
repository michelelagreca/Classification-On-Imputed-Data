# Classification on imputed data
This project was part of the exam and of the evaluation of the course 'Data and Information Quality' at Politecnico di Milano. 

Missing values are an important element to deal with when it comes to work with Machine Learning
and in general with data. The presence of missing data may become a problem since the information
are likely to be biased on the smaller amount of data. Moreover, ML methods suffer missing value since
they don’t accept null value, and also because they work well when a lot of data are available. 

The
project aims to build a case study on the comparison between different types of imputation techniques,
as well as measuring the performances of two ML algorithms for classification trained and evaluated
on a dataset that each time has a bigger rate of missing values imputed.

## Data
The dataset is composed of 3017 records, each having 15 features. Initially, the completeness of the dataset is 100%, and the dataset does not have any missing value.
Five additional dataset has been created from the complete one: one having 10% of missing values,
one having 20% of missing values, one having 30% of missing values, one having 40% of missing values,
one having 50% of missing values. The missing values have been inserted completely at random.

## Imputation techniques
Exploring the variables, the values that each attribute assumes, and at the cardinality of each value,
it is possible to choose how to treat each attribute for the standard imputation: median imputation will be used (keeping it without decimal values) for numerical variables, bfill, ffill or the mode for the categorical variables. 

Advanced imputation will be also used: it will be done using MICE - Multiple Imputation by Chained Equations. For numerical variables KNN will be used, while for categorical variables Decision Trees will be used.

For the imputation accuracy assessment, the accuracy for the categorical variables will be the number of the correct imputed values over
the number of elements of that variable, while the accuracy for the numerical variables will be calculated as the cosine similarity between the
imputed and the original one.

## Machine learning algorithms
Since we have a classification problem, Logistic regression and Support vector machine (SVM) will be used. To evaluate the performances of the chosen method, the confusion matrix will be calculated, as well as Accuracy, Precision, Recall and F1 score.

