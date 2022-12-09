# Classification on imputed data

The goal of the project is to explore different imputation techniques to use when missing values are present.

Starting from a cleaned and complete dataset, 5 additional datasets will be created: the first with the 50% of missing values, the second with the 40% of missing values, the third with the 30% of missing values, the fourth with the 20% of missing values and the fifth with the 10% of missing values.

For each dataset, a standard and an advanced imputation technique will be used, measuring the similarity between the imputed datasets and the original one. Lastly, logistic regression adn SVM will be applied to solve a classficiation problem of this data, using the original dataset and the imputed datasets, and looking at the differences in performances that can be due to the missing values and to the imputed techniques used.
