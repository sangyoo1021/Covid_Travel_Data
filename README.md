# Final Project 

## Airline travel and covid-19


## Project Overview
Given the current pandemic ongoing in the world, the team decided to analyze the domestic airline travel and its correlation with Covid-19. The team will test data points and correlation between Covid-19 cases, vaccine, and number of passengers traveling domestically via airplanes. Additionally, the team is hoping to find a correlation between vaccines and post-pandemic traveling. The team will create a model, train the model, and create predictions for future trends by using the historical values of traveling for the past three years.

## Links
* [Dashboard](https://public.tableau.com/app/profile/nick.emery/viz/Covid_TravelData/TotalCases?publish=yes)
* [Presentation](https://docs.google.com/presentation/d/1BG5ym9iFnZlSlqdPJViYNIFEAI0LnRnIBuntDVDaSYQ/edit?usp=sharing)

## Communication protocols
* Throughout this project, the team used Slack app regulary to communicate with each other.
* The team used Zoom for video calls and screen sharing twice a week.
* The team used Github platform to work together on this project.

## Team members and roles
* Eno Vaqari - Triangle Role
* Nick Emery Circle Role
* Sang Yoo - Square Role

### Data Sources

* https://ourworldindata.org
  * Covid data
* https://www.transtats.bts.gov
  * Passangers data
* https://www.tsa.gov/coronavirus/passenger-throughput
  * Travel Data
  
*     ERD
![ERD Diagram - Initial Build](https://user-images.githubusercontent.com/98061420/173248159-a223498c-5451-4b34-995b-0ccc56a7d7cb.PNG)

![Joined MasterTable](https://user-images.githubusercontent.com/98061420/175851507-c77dd26c-dd61-4966-8664-ba672740d746.PNG)


## Analysis and Machine Learning 

The team retrieved data for US air travelers and Covid 19 cases, and replaced all the Null values of Covid 19 cases prior to late 2019 with 0. Once the data was ready, used Linear regression and Random Forest models to analyze the data and store information specific to the dataset. The models were used to predict the future trends of air travel using historical values of the past three years, considering the effects of Covid-19 cases and vaccines. The team selected 2 different models to compare the accuracy scores, efficiency, and optimal results. Linear Regression is easy to implement and interpret, and efficient to train. Random Forest Classifier handles thousands of input variables without deletion and runs efficiently on large datasets.
The team used test_train_split to split the data and stored 1.data in X and 2.target in Y. By passing the test_size as 0.25, the team classified 25% of data in test part and 75% in train part. Additionally, random_state is set as 1, which guarantees that the same sequence of random numbers is generated each time the code is ran. Finally, the team printed the shape of train data. 
Next steps involved creation of StandardScaler, instances_Scaled the data and fitted the model. Once the model generated predictions, the team created data frame with both prediction and actual scores for both models chosen. 
Linear Regression model generated a R squared value of 61% and the Random Forest Classifier generated a R squared value of 86%, resulting in the Random Forest Classifier as the most accurate and better prediction model.

![https://github.com/sangyoo1021/Covid_Travel_Data/blob/main/PNGs/Lr.png]
![https://github.com/sangyoo1021/Covid_Travel_Data/blob/main/PNGs/Screen%20Shot%202022-07-03%20at%2010.45.45%20PM.png]

The model could be further enhanced by including ticket pricing, travel limitations, and other external factors.

