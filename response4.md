## Data Science Reflection 4

### Predicting Customer Retention using Churn Prediction Models

An important aspect of Data Science is building models that can predict future behavior. In particular, churn prediction can be valuable in increasing customer retention for 
businesses. **Customer churn** occurs when a customer stops doing business with a company or stops using their product. Streaming services, telecommunication companies, and 
other businesses that rely on periodic subscriptions benefit from looking closer into the data produced by customers. 

When creating a churn prediction model, it is important to import and clean the data, analyze the data, and do feature engineering. To refine the data, unwanted rows or columns
can be removed. This includes unneeded or missing data that is not beneficial to forming a model. Next, it is necessary to analyze the data. Depending on the context of the 
dataset, one can start to identify valuable pieces of data. For “Sparkify”, a fictitious music streaming service containing realistic data provided by Udacity Data Science,
instances of “thumbs down”, “error”, visiting the help page, and the number of songs played proved to be important. To analyze the data, Udacity determined whether the number 
of songs played daily increased or decreased quarterly. In another example using data from Telco Customer Churn, data scientists studied the correlation between the churn rate 
and a number of different variables, including gender, internet service, type of contract, payment method, and use of Tech Support, all of which are categorical features. 
**Categorical features** are that which have value without order, while **numerical features** are based solely on numbers. While categorical features use often use bar plots 
during analysis to indicate a correlation, numerical features can use scatterplots to determine a pattern. Some numerical features for the Telco dataset include tenure, monthly
charges, and total charges. 

During the process of feature engineering, both numerical and categorical data can be clustered to gain more insight and prepare the features to be used for a model. When
clustering categorical data, integers are assigned to values. For example, 0 may be assigned to male and 1 to female for data relating to gender. Finally, to create a robust
model that may be used to predict customer churn, one must find the variables that make customers more or less likely to churn. From a logistic regression model, the 
**p-value**, a probabilistic reference value, can be used to indicate the significance of variables. If the p-value of a predictor is less than 0.05, the variable is considered significant. For Telco’s dataset, senior 
citizen status, having DSL internet service, and a lack of online security was found to be most significant. However, the main indicators of other datasets differed to include
the type of contract, tenure, and total charges. From this, a classification model or a decision tree can be formed with the most important variables to predict customer
churn. 

Though both models were somewhat successful in predicting customer churn, they could be improved with the addition of more data or a resampling of data. Though our world is
everchanging, studying data from the past can help predict what’s to come in the future. In this way, Data Science is increasingly important in our modern world.


#### References

Karaman, Baris. Churn Prediction. 15 September 2019, https://towardsdatascience.com/churn-prediction-3a4a36c2129a.

Orac, Roman. Churn Prediction. 9 October 2020, https://towardsdatascience.com/churn-prediction-770d6cb582a5.

Svitek, Matej. Music Streaming Service Churn Predictions with PySpark. 27 October 2020, https://mt-svitek.medium.com/music-streaming-service-churn-predictions-with-pyspark-b4c788ac0c5b.

