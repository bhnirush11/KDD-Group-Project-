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

## Evaluation

## Conclusion

For future work, this project can be added with more features making the dataset more rich in features. 

## Future Enhancements
- We will compare the performances of various machine learning algorithms and identify the algorithm that gives the best result on flight delay dataset. 

## Tasks for Deliverable 2

- [x] Introduction to Problem or Opportunity (include supporting domain information)
- [x] Research Question(s)
- [x] Data Resources
- [x] Date Preprocessing
- [x] Data Understanding and Exploration
- [x] Data Preparation for Modeling
- [ ] Modeling
- [ ] Evaluation
- [ ] Results
- [ ] Future Work

 




