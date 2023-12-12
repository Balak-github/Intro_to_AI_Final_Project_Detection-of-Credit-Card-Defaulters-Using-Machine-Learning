# Introduction to Artifical Intelligence - Final Project   (Detection of Credit Card Defaulters Using Machine Learning)
This is the final project for Artificial Intelligence course, CSCI-6660-02 done by Bala Venkata Yaswanth Kommuru (00787234), Prathima Chowdary Tummala (00791386), Sai Tarun Reddy Pappu (00802951)

This project involves training a data set with various machine learning techniques and assessing the effectiveness of each model to identify credit card defaulters.

## List of Contents:
+ Data Set
+ Machine Learning models used
+ How we used these models in project
+ Performance

## Data Set
This dataset includes data on missed payments, demographic factors, credit data, payment history, and bill statements for credit card users from April to September 2005.

There are 24 features to choose from:

### Demographic Information
+ ID: ID of each client
+ LIMIT_BAL: Amount of given credit in NT dollars (includes individual and family / supplementary credit)
+ SEX: Gender (1=male, 2=female)
+EDUCATION: (1=graduate school, 2=university, 3=high school, 4=others, 5=unknown, 6=unknown)
+ MARRIAGE: Marital status (1=married, 2=single, 3=others)
+ AGE: Age in years

### Repayment Status for past 6 months

### (-1 = pay duly, 1 = payment delay for one month, 2 = payment delay for two months, ..., 9 = payment delay for nine months and above)

+ PAY_0: Repayment status in September, 2005
+ PAY_2: Repayment status in August, 2005 (scale same as above)
+ PAY_3: Repayment status in July, 2005 (scale same as above)
+ PAY_4: Repayment status in June, 2005 (scale same as above)
+ PAY_5: Repayment status in May, 2005 (scale same as above)
+ PAY_6: Repayment status in April, 2005 (scale same as above)
  
### Amount of bill statement for past 6 months

+ BILL_AMT1: Amount of bill statement in September, 2005 (NT dollar)
+ BILL_AMT2: Amount of bill statement in August, 2005 (NT dollar)
+ BILL_AMT3: Amount of bill statement in July, 2005 (NT dollar)
+ BILL_AMT4: Amount of bill statement in June, 2005 (NT dollar)
+ BILL_AMT5: Amount of bill statement in May, 2005 (NT dollar)
+ BILL_AMT6: Amount of bill statement in April, 2005 (NT dollar)

### Amount of previous payment for past 6 months

+ PAY_AMT1: Amount of previous payment in September, 2005 (NT dollar)
+ PAY_AMT2: Amount of previous payment in August, 2005 (NT dollar)
+ PAY_AMT3: Amount of previous payment in July, 2005 (NT dollar)
+ PAY_AMT4: Amount of previous payment in June, 2005 (NT dollar)
+ PAY_AMT5: Amount of previous payment in May, 2005 (NT dollar)
+ PAY_AMT6: Amount of previous payment in April, 2005 (NT dollar)

### Target Variable

+ default payment next month: Default payment (1=yes, 0=no)

## Machine Learning models used

### SVM

Support vector machines (SVMs), a form of supervised machine learning technique, can be utilized for both classification and regression tasks. It is, however, most commonly employed to address categorization concerns. Each value in the SVM algorithm is associated with a specific location. Make a point in n-dimensional space (n is the number of features) that represents the value of each piece of information. Find a super plane that clearly separates the two classes, and then classify them.

### How it works

A straightforward linear SVM classifier operates by tracing a straight line between two classes. In other words, all the data points on one side of the line correspond to a category, whereas the data points on the other side of the line are assigned to different categories. This implies that you can choose from an endless number of lines. The linear SVM algorithm chooses the optimum line for classifying data points, making it preferable than other techniques like closest neighbor. Select a line to divide the data, keeping it as far away from the cabinet data points as you can. If you utilize 2D examples, all machine learning jargon will be simpler to comprehend. A grid usually contains multiple data points. These data points need to be categorized, but you don't want to categorize them wrongly. This indicates that the line separating the other data points from the two closest points is what we're looking for. As a result, the reference vector for identifying this line is provided by the two nearest data points. This line is known as the decision boundary.

### Logistic Regression

Logistic regression, often known as logit regression, binary logit, or binary logistic regression, is a type of statistical analysis. The logistic regression statistical method forecasts the outcome of a dependent variable using previous data. It is a type of regression analysis commonly used to solve binary categorization problems. Logistic regression is used to model the log of the outcome's odds ratio. The coefficients of a logistic regression model are obtained via maximum likelihood estimation. This is because, unlike linear regression, there is no closed-form solution. Regression analysis is a form of predictive modeling technique used to determine the relationship between one or more independent variables and a dependent variable.

### How it works

We fit a "S" shaped logistic function in logistic regression instead of a regression line, which forecasts two maximum values (0 or 1). The logistic function's curve depicts the likelihood of many outcomes, including whether the cells are malignant, whether or not a mouse is obese based on its weight, and other outcomes. Logistic regression is a crucial machine learning technique because it can produce probabilities and classify new data using both continuous and discrete datasets. Observations can be categorized using a variety of types of data using logistic regression, which can also quickly pinpoint the most beneficial parameters for categorization.

### Naive bayes

To carry out classification tasks, a Naive Bayes classifier, a probabilistic machine learning model, is used. The classifier's foundation is the Bayes theorem.

### How it works

Using Bayes' theorem, we may determine how likely it is that A will occur if B has already happened. The hypothesis is A, and B is the proof. In this instance, it is assumed that the predictors and features are independent. In other words, the presence of one trait does not affect the other. It is hence referred to as naive.

### Random Forest

Random forest is a supervised learning algorithm. It assembles decision trees, which are commonly trained using the "bagging" method, into a "forest." The bagging approach's key tenet is that the output is improved by combining different learning models.

Random forest can address classification and regression problems, which are common in modern machine learning systems. Let's look into random forest in categorization because it's commonly thought of as the cornerstone of machine learning.

The hyperparameters of a decision tree or bagging classifier are similar to those of a random forest. Fortunately, rather than combining a decision tree with a bagging classifier, you may use the classifier-class of a random forest. Use the algorithm's regressor to handle regression jobs using random forest.

As the trees grow, the random forest improves the model's randomness. When dividing a node, it selects the best feature from a random selection of features rather than focusing on the most significant feature. As a result, there is more diversity, which leads to a better model.

As a result, the method for dividing a node in random forest only takes into account a random subset of the features. Trees can be further randomized by utilizing random thresholds for each characteristic rather than striving for the highest achievable thresholds (like a standard decision tree does).

## How we used these models in project

+ Performed training on data set.
+ Predicting the model by using test data set.
+ Evaluated the model by using F1 score,K Fold Cross validation and confusion matrix.
+ Testing the trained model with new dataset

## Performance

<img width="461" alt="236108379-2d8e973a-e91f-4f15-b7ad-be60b7bc5666" src="https://github.com/Balak-github/Intro_to_AI_Final_Project_Detection-of-Credit-Card-Defaulters-Using-Machine-Learning/assets/67410758/1398d44f-8ec0-4575-8a49-1b28e6418627">

![236108731-e05834ce-6711-46c8-9c07-c581a671f539](https://github.com/Balak-github/Intro_to_AI_Final_Project_Detection-of-Credit-Card-Defaulters-Using-Machine-Learning/assets/67410758/e4528454-080c-4f50-9f52-5fa1059a3740)

