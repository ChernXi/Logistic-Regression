# Logistic-Regression

The logistic regression model is mainly used for binary classification. <br>
The logistic regression model is not just another model to use, but when you apply it correctly, it can outperform even the much more complicated dense neural network. <br>
Before we dig into it, I will show you an example where it is best to use Logistic Regression: The Titanic survival prediction model <br>
If you use a multinomial regression model, you can basically get an accuracy of around 74%. <br>
If you use a dense neural network model, you can enhance the accuracy to 82%. (By considering the deeper relationship between the basic attributes.) <br>
Guess what accuracy we get by using a Logistic Regression model? We can make it to 95%!!! <br>
To see how it was done, you can take a look at [Titanic Survival Logistic Regression Model](https://github.com/ChernXi/Logistic-Regression/blob/e77cb08ead4a2f091c353d5fb0c33aa84f85ea42/Titanic%20Survival%20Logistic%20Regression%20Model.ipynb). <br>

## When to use?
Logistic Regression is best to use to classify binary labels from many continuous features. It can also be used when the features are not continuous.

## Logic of logistic regression
In short, logistic regression is a pipeline of normalized multinomial regression followed by a classification using the Sigmoid Function.
Naively speacking, it does a regression, then labels them based on the results.

## Why it is more accurate in classification?
Firstly, no information is suppressed prior to training.
Unlike those classification methods that reduce the numerical features to classified features, logistic regression preserves the original information completely to do training.<br>

Secondly, It have a large margin of error.
Other classification method just outcome with one result(except Random Forest which used many result to vote for the final result), they can be either correct or wrong for a binary classification problem. BUT, Logistic regression can predict a regression wrongly, but still classify them correctly.
Logistic regression take all result from $0^+$ to $+/infinity$ as True and all result from $0^-$ to $-/infinity$ as False.
Imagine, it could be a bad result for regression if the actual value is 100000 but the regression model predict it as 1.
However, after doing classification, they belongs to the same group and therefore result in a CORRECT prediction.<br>


