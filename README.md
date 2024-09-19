# Data-Analysis-Titanic-Data-
Report on Titanic Dataset Analysis
The goal of this analysis is to apply various Data Analysis Techniques such as Logistic Regression, K-means Clustering, and Decision Tree Regressor to explore the Titanic dataset and derive meaningful insights about passenger survival and other features.For that the following steps were followed.
Data Loading and Cleaning: I have loaded  the Titanic dataset and handled  missing values in 'Age', 'Fare', and 'Embarked' columns.In Age column I have filled the missing value with the median value also for the fare column.
Exploratory Data Analysis: Visualizing data using a correlation heatmap and distribution plots to understand feature relationships and survival patterns.
Feature Engineering: Converting categorical variables like 'Sex' and 'Embarked' to numerical representations.
Model Training: Training a logistic regression model to predict survival based on selected features.
Model Evaluation: Evaluating the logistic regression model's performance using accuracy and a confusion matrix.
Statistical Evaluation: Tried to evaluate and understand the significance of the predictors and model overfitting tendency in the regression model. 
Clustering: Applying KMeans clustering to group passengers based on features like 'Fare' and  'Age'
Decision Tree Regression: Using a decision tree regressor to predict passenger fares based on other features and visualizing the tree and calculate the RMSE value to evaluate the model 

Method: Logistic Regression was applied to predict whether a passenger survived the Titanic disaster based on features such as 'Pclass', 'Sex', 'Age', 'SibSp', 'Parch', 'Fare', 'Embarked'
Key Findings:
Accuracy: The logistic regression model achieved an accuracy of around 100%.
Interpretation: The model received perfect accuracy which means it classified and predicted all 84 instances correctly.
Visualization: A confusion matrix was generated to show the classification performance, with clear differentiation between survived and non-survived passengers.where 1 represent survived and 0 represent did not survive.  

Statistical Findings 
After getting 100 percent accuracy it indicates it is a overfitted model and can be misleading logistic regression and if we notice that only the Pclass’s p value is it's still statistically significant, suggesting that the passenger's class is a significant predictor of survival and other are not significant as the p value is very high. 
And it predicted Complete Separation: The results show that there is complete separation or perfect prediction.
In this case the Maximum Likelihood Estimator does not exist and the parameters
are not identified.


Fig: Logistic Regression statistical analysis 

2. K-means Clustering: Passenger Segmentation
Method: K-means clustering was used to segment passengers based on features like Age and Fare and Pclass where 1 = First class 2 = Second class 3 = Third class.
Key Findings:
Clusters: The optimal number of clusters chosen was 3, based on the elbow method. These clusters represented different groups of passengers:
Cluster 1: Younger passengers with lower fares.
Cluster 2: Middle-aged passengers with moderate fares.
Cluster 3: Older passengers with higher fares.
Interpretation: This clustering reveals distinct patterns among passengers, with fare and age playing a major role in grouping them. Higher fare often correlates with higher-class tickets, and indirectly, better survival rates.
Visualization: pair plots were used to visualize the clusters.


3. Decision Tree Regressor: Predicting Fare
Method: A Decision Tree Regressor was applied to predict the Fare based on features such as Pclass, Age, and Embarked etc.
Key Findings:
Root Mean Squared Error (RMSE): The RMSE of the Decision Tree model was 35.583567611840074, The RMSE value of approx 35.6 means that, on average, the predictions are off by approximately 36.6 units from the actual values.
Important Features:
Pclass: The most significant factor in determining fare, with first-class passengers paying substantially more.
Age: Older passengers tended to pay slightly higher fares.
Interpretation: The decision tree effectively identifies the hierarchical importance of class and age in determining the fare, with wealthier passengers (higher Pclass) paying more.
Visualization: The decision tree structure was plotted to illustrate the splits and importance of each feature.

Here we can see that people whose age is greater than 57.5 tends to pay the higher ticket fare value which is 229.482 and the Higher class people tend to pay the higher ticket fare.
Conclusion:
I have tried to use the combination of logistic regression, K-means clustering, and decision tree regression to provide a comprehensive analysis of the Titanic dataset. The analysis highlights the impact of socio-economic status on survival during the disaster, while clustering offers a data-driven way to segment passengers into meaningful groups.

Submitted By 
Tawhida Bintay Kabir
