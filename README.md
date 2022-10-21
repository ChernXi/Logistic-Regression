# Logistic-Regression

The logistic regression model is mainly used for binary classification. <br>
It can provide us with quick classification results that are usually quite accurate (marginally inferior to DNN).<br>
To see how it was done, you can take a look at [Titanic Survival Logistic Regression Model](https://github.com/ChernXi/Logistic-Regression/blob/e77cb08ead4a2f091c353d5fb0c33aa84f85ea42/Titanic%20Survival%20Logistic%20Regression%20Model.ipynb). <br>

## When to use?
Logistic Regression is best to use to classify binary labels from many continuous features. It can also be used when the features are not continuous.

## Logic of logistic regression
In short, logistic regression does a normalized multinomial regression followed by a classification using the Sigmoid Function.
Naively speacking, it does a regression, then labels the result.

## What are the advantages of Logistic Regression in Classification?
#### Firstly, no information loss prior to training.
Unlike those classification methods that reduce the numerical features to classified features, logistic regression preserves the original information completely to do training, so it can capture more information during the training. <br>

#### Secondly, It has a large tolerance of error.
Logistic regression can produce a bad regression result, BUT still classify them correctly.<br>

Logistic regression take all result from $0^+$ to $+\infty$ as True and all result from $0^-$ to $-\infty$ as False.<br>
Imagine, it could be a bad result for regression if the actual value is 100000 but the regression model predict it as 1.<br>
However, after doing classification, they belongs to the same group and therefore result in a CORRECT prediction.<br>


