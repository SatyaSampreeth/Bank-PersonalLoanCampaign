# Bank-PersonalLoanCampaign
#**Project** :
Objective: The retail marketing department to devise campaigns with better target marketing to increase the success ratio with minimal budget.The department wants to build a model that will help them identify the potential customers who have higher probability of purchasing the loan. This will increase the success ratio while at the same time reduce the cost of the campaign.

The dataset contains data on 5000 customers

**Variables definition**

ID - Customer ID

Age - Customer's age in completed years

Experience - Number of years of professional experience.

Income - Annual income of the customer (in $ 1000).

ZIPCode - Home Address ZIP code

Family - Family size of the customer
CCAvg - Avg. spending on credit cards per month - in thousands usd

Education - Education Level of the customer.

Undergrad
Graduate
Advanced/Professional
Mortgage - Value of house mortgage if any - in thousands used
Personal Loan - Did this customer accept the personal loan offered in the last campaign?(This is our target variable)
Securities Account - Does the customer have a securities account with the bank?
CD Account - Does the customer have a certificate of deposit (CD) account with the bank?

Online - Does the customer use internet banking facilities?

CreditCard - Does the customer uses a credit card issued by Bank?

**Model Observation**

The accuracy metric which is the overall model's peformance i.e. not class specific, can be misleading
So,when the target classes are extremely skewed (i.e. do not have same no of samples). We should always use the recall and precision metric.
Recall is, how many records of a class were correctly identified as belonging to that class.i.e. True Positive / (True Positive + False Negative)
Precision is how many records identified as belonging to class 1 truly belong to class 1 i.e. True Positive / (True Positive + False Positive)
So we should make sure that our model peforms well on these metrics for all the classes, especially for the classes which have lower representation in the skew

*Best Model- Conclusion*

Seven classification algorithms were used in this study.
The logistic Regression model has the accuracy 0.91 which is low compared to others.
The KNN is distance based which not perfect for this situation.Though the accuracy is ok(0.91) but confusion matrix tells that is correct predictions is not that much acceptable
The Naive Bayes giving the accuracy less in comaprision to other models meaning the probability of determing the target correctly is less.
It seems like Decision Tree algorithm have the high accuracy(0.98) and we can choose this as our final model,but it doesn't have good precision and recall values for class 1.
It has a high accuracy(0.99) compared to all the other models but it has slightly high recall value for class 1 compared to others,which is not so good to confirm the model as Random Forest.
Though Bagging Classifier gives high accuracy(0.98) and comparatively less recall value than Random Forest.It has comparatively less precision than others which doesn't make to selct it.
And the final classifier used is Voting Classifier which is a collection of several models working together on a single set is called an ensemble. The method is called Ensemble Learning. It is much more useful, uses all different models rather than any one.
Lower error
Less over-fitting
Taste great
Has good accuracy of 0.985 and high precision and low recall values for class 1 so,can select as the final model for the classification and prediction for the bank in campaigning for Personal Loans

The aim of the bank is to convert there liability customers into loan customers

They want to set up a new marketing campaign; hence, they need information about the connection between the variables given in the data.

The Voting Classifier model is the best as the accuracy of the train and test set is almost similar and also the precsion and recall accuracy is good. The confusion matrix is also better in comparision to other models.
