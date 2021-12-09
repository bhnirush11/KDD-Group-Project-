# Understanding Flight Delays - KDD Group 9

## Team Members

- MEGHANA MADUGULA
- NIRUSH REDDY BHIMIREDDY
- SANJANA MADUGULA
- SAYEESH DARSHAN KANALA

## Project Objective
- Flight delays are a modern-day problem. Passengers, airlines, and airports all suffer from these delays, which are inconvenient and costly.
- This project analyzes flight delay data in order to gain a better understanding of how commercial aviation operates and to anticipate when delays are likely. 

## Research Questions
1) How is the amount of time spent by the flight between Taxi out and wheels off affecting the estimated time of arrival? 
2) On what days of the week and a particular time during that day do we observe the maximum delays in flight time?
3) While considering landing delay (at destination), how is flight air time affecting delay time?
4) Analyzing reason for delay(weather delay, technical delay, logistics delay, airline traffic) w.r.t delay time, airline, airport?

## Data and Source Description

- https://www.bts.dot.gov/explore-topics-and-geography/topics/understanding-reporting-causes-flight-delays-and-cancellations-0
- Dataset : https://drive.google.com/file/d/1X3wuFlxQ8Takyu-aMpnuQjop1yjVf_tA/view?usp=sharing

  The datasest contains features such as Scheduled Departure, Departure Time, Departure Delay, Taxi Out, Air Time, Arrival Time, Arrival Delay, Reason for Delay,     etc.
  
## CRISP-DM Process:

Cross-industry standard process for data mining, known as CRISP-DM, is an open standard process model that describes common approaches used by data mining experts. It is the most widely-used analytics model.

This model is an idealised sequence of events. In practice many of the tasks can be performed in a different order and it will often be necessary to backtrack to previous tasks and repeat certain actions. The model does not try to capture all possible routes through the data mining process. CRISP-DM breaks the process of data mining into six major phases:

- Data Understanding
- Data Preparation
- Machine Learning
- Evaluation

## Following datasets are considered :

airlines.csv

airports.csv

flights.csv

airlines: Dataset contains airlines along with their codes

airports : Dataset contains location details of the respective airports that are considered

flights: Dataset contains features which are the details captured 

## Data Preparation/Preprocessing:

- Importing all the required modules
- Loading the datasets(airlines,airports and flights)
- Understanding information provided in the datasets and looking for types of columns and any missing values
- Checked for null values in all the datasets
- To avoid any issues, we dropped the columns having null values
- Analysed the data by performing EDA on the dataset. We used different vizualization techniques

 <img width="705" alt="Screenshot 2021-11-17 at 11 37 31 PM" src="https://user-images.githubusercontent.com/91857002/142352759-2dd5f1de-a13c-4045-8d65-f02cbe0c2821.png">
 
 - Distribution of flights in the dataset across airlines 

<img width="1057" alt="Screenshot 2021-11-17 at 11 41 22 PM" src="https://user-images.githubusercontent.com/91857002/142353025-a2e6b172-5b51-4242-baca-d7fa30a92efb.png">

## Machine Learning
After the data pre-processing phase, we have implemented the following supervised learning algorithms to make the predictions for Flight Delays. 

Model 1: 
Logistic Regression is used to predict the probability of a target variable.

R-Squared value This value ranges from 0 to 1. Value ‘1’ indicates predictor perfectly accounts for all the variations in Y. Value ‘0’ indicates that predictor ‘x’ accounts for no variation in ‘y’. 
- Accuracy obtained : 0.9308

Model 2: 
Decision Tree algorithm is used to create a model that predicts the value of a target variable, for which the decision tree uses the tree representation to solve the problem in which the leaf node corresponds to a class label and attributes are represented on the internal node of the tree.
- Accuracy obtained : 0.8860

Model 3: 
Random Forest algorithm builds multiple decision trees and merges them together to get a more accurate and stable prediction.
- Accuracy obtained : 0.9331

Model 4: 
Naïve Bayes is a simple learning algorithm that utilizes Bayes rule together with a strong assumption that the attributes are conditionally independent, given the class. 
- Accuracy obtained : 0.8195

## Evaluation

The evaluation metrics used are :
- Accuracy : Accuracy is the number of correctly predicted data points out of all the data points.

- Precision: Precision measures how many observations, both positive and negative, were correctly classified.

- Recall : The recall is the measure of our model correctly identifying True Positives.

- F1 Score : The F1 score is defined as the harmonic mean of precision and recall.

- AUC curve : AUC score measures the total area underneath the ROC curve.

- Kappa metric : Kappa metric expresses the level of agreement between two annotators on a classification problem.

Flight Delays data set is analyzed in this project. Considering the evaluation metrics of all the models, we can conclude that 'Random Forest' performs well on our dataset to predict flight delays.

## Conclusion
Flight Delays is the data set we have analyzed in this project. We have implemented various visualization techniques to understand our data better and find the relation between different attributes of the dataset. The unique thing that we found out about our dataset after performing modeling is that it showed high precision value with all the modeling techniques. We can say that the dataset is unbalanced since it had more 0's than 1's in our result column. Attributes like Cancellation reason, air system delay, security delay, airline delay, late aircraft delay and weather delay had the hightest number of null values. We handled some of these null values using imputation and the others by replacing them with central measures of tendancy. Later on, we have visualized the correlation between all the attributes, and dropped the features with the least correlation with other features. We have added a result column to store the predicted result, the result we predicted is the airline delay. We have used Logistic Regression, Decision, Random Forest, Naive Baiyes for evaluation. Considering the evaluation metrics of all the models, we can conclude that 'Random Forest' performs well on our dataset to predict flight delays. One of the main problems we faced while performing modelling was the runtime of each algorithm. Since the number of records in our dataset is very large, the algorithms took very long to run. Another challenge we faced was identifying the algorithm that performed best on our data. The accurancy score of every algorithm was fairly equal, we had to consider other values like the F1 score and Area Under the Metric to identify the algorithm that performed best.




## Future Scope
- Airport level dataset in terms of number of runways, capacity of airport can be helpful
- We can forecast arrival delay even without including departure delay as an attribute if weather and air traffic control information are made available. We can also estimate whether a flight will be delayed or cancelled depending on weather factors such as snow, rain, or storms.


