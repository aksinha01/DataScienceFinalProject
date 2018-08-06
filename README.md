## DataScienceFinalProject
DataScience Final Project for 3250

### Project Description - Telecom Churn Analysis 

1. Data Preparation and Pre-prediction Analysis
a. Explore Data
b. Find statistics
b. Apply cluster analysis/Time series analysis and other methods you learned on data
2. Predictive Modeling (Classification) 
a. Classification using Decision Tree 
b. Classification using Naive Bayes
c. Choose one another classification algorithm of your choice, apply and describe it
d. Compare the results of the 3 techniques
3. Conclusions and Recommendations
Data Preparation and Pre-prediction Analysis

The first and foremost step of data mining process is to understand the data and identify the research question(s). Here are some suggestions to explore and understand datasets:

Look at the attribute type; e.g., categorical, ordinal or quantitative.
Find max, min, mean and standard deviation of attributes.
Determine any outlier values (records) for each of the attributes or attributes under
consideration (min, max, std. dev, scatter plots, box plots or others can be used).
Analyze the distribution of numeric attributes (normal or other). 
Plot histograms for attributes of concern and analyze whether they have any influence on the class
Try to answer these questions by different visualization techniques:
Which attributes seem to be most linked to the class attribute?
Which attributes do you think can be eliminated or included in the analysis?
Phone number
Determine whether the dataset has an imbalanced class distribution
proportion of records of different types or not).

### Predictive Modeling (Classification)

After an overall understanding about the dataset, you can use classification algorithms, Decision Tree and Naïve Bayes. Also, choose a classification algorithm of your own choice, explain it a at a high level and compare your results
You will predict the class attribute by using each classification algorithm.

Determine the right strategy for dataset split: simple training or testing, 10-fold cross validation, 3-fold cross validation, etc.

Repeat the same process for Decision Trees, Naïve Bayes and the third classification algorithm of your choice.
Determine your performance measures (accuracy, recall, etc.).
Identify which algorithm performs well and in which settings.
	

### Conclusions and Recommendations
State your major findings from different sections. State your recommendation to the company that they can put into place to solve their problem.


Churn Dataset

Customer churn or customer attrition means the loss of customers for a company. The
problem for customer churn is that the company would like to know in advance which
customers would churn in near future. You are a member of a team of data scientists and
the task of your team is to help this company in characterizing customer churn through data
analytics methods. This dataset has 21 attributes including a binary class attribute about
churn. The descriptions of the attributes are given below:

1. State: Customer’s state.
2. Account Length: Integer number showing the duration of activity for customer account.
3. Area Code: Area code of customer.
4. Phone Number: Phone number of customer.
5. Inter Plan: Binary indicator showing whether the customer has international calling plan.
6. VoiceMail Plan: Indicator of voice mail plan.
7. No of Vmail Mesgs: The number of voicemail messages.
8. Total Day Min: The number of minutes the customer used the service during day time
(continuous quantitative data type).
9. Total Day Calls: Discrete attribute indicating the total number of calls during day time.
10. Total Day Charge: Charges for using the service during day time (continuous data
type).
11. Total Evening Min: The number of minutes the customer used the service during
evening time.
12. Total Evening Calls: The number of calls during evening time.
13. Total Evening Charge: Charges for using the service during evening time.
14. Total Night Min: Number of minutes the customer used the service during night time.
15. Total Night Calls: The number of calls during night time.
16. Total Night Charge: Charges for using the service during night time.
17. Total Int Min: Number of minutes the customer used the service to make international
calls.
18. Total Int Calls: The number of international calls.
19. Total Int Charge: Charges for international calls.
20. No of Calls Customer Service: The number of calls to customer support service.
21. Churn: Class attribute with binary values (True for churn and False for not churn).

How to Compare Your Classification Models (Model Selection)

In order to evaluate and compare machine learning models with different features, a known
approach is to create a baseline model first. This can be done by training one model (e.g.,
decision tree) on the training set using the entire feature set (all attributes) and evaluating its
performance using the selected metric (such as accuracy, true positive rate, false positive rate,
etc.) on the validation set (or test set). Optimization of the model parameters or selection of
features could be done by changing one variable (e.g., one parameter or one feature) at a time
and re-training the model on the same training set. Finally, one needs to compare the
performance of different models built using different features on the same validation set (or
test set). This would give an indication whether that variable (feature or parameter) has
increased or decreased the performance.

1. Using 3-ways data splitting (Here, you will have to divide a dataset yourself or find a library/function in Python):
• Training (e.g., 60%): for training the model
• Validation (e.g., 20%): for evaluating and comparing the performance after varying
parameters, features, etc. In addition, this is used for selecting the “best” model.
• Testing (e.g., 20%): only used at the end to evaluate the final performance and report
the results of the selected models (best performing models from the above step)
• This video describes this approach: https://www.youtube.com/watch?v=4wGquWG-vGw

2. Using 10-fold cross validation (10-FCV) on the entire dataset:
• Create the base model by train and evaluate its (average) performance using 10-FCV.
• Change model parameters or features, retrain and re-evaluate the (average) model
performance using the 10-FCV strategy.
• Report the results of best performing models (using the best parameters and features
select from the above step).

