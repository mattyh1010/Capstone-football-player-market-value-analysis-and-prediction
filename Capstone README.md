
# Football Player Market Value Analysis and Predictive Model

A data science project to predict market values of football players


## The Business Problem and Objectives

The football transfer market is a forever growing and seemingly ludicrous place, where players are being bought for excessive and inflated prices due to the increasing influence of wealth in the game. 

As not all football clubs around the world have equal resources available to compete with each other, it is becoming increasingly important for so-called ‘lesser’ clubs to find more creative and scientific ways to find value in the market so they can continue to compete with the more wealthy clubs. 

The objective of my project is to create a model that predicts the Market Value of football players and attain a list of players who represent the best value in terms of my model compared to their actual Market Value, therefore finding players who may represent good value compared to other players in the market. This would allow clubs with less financial power to bridge the gap to using a data science approach.

## Solution Strategy

The solution to this problem will be the development of a data science project. This project will use a machine learning model which will predict football player market values to be compared to actual market values.

Step 1 - Data Collection: In this section I will need to find data that is appropriate for me to achieve the objective of the project. This will require a database of players that includes information about their position, age, nationality, market value and stats or attributes.

Step 2 - Data Cleaning: In this section I will analyse the format and characteristics of the data acquired in order to prepare it for analysis and modelling. This stage will include checking my data for any null values and deciding on how to best handle them should they be there, checking for and removing duplicates, and lastly checking and changing data types if necessary.

Step 3 - Exploratory Data Analysis: In this section I will analyse distrubutions of my data to inform data wrangling and feature engineering. I will then aim to analyse the demographic nature of the target variable (Market Value). I will explore the distributions of market value in terms of player age, player position and player nationality, to understand where market value is distributed throughout the data acquired.

Step 4 - Data Preparation: In this section the data will be prepared for the machine learning model. This will include data wrangling and feature engineering/selection to correctly format it for modelling, ensuring optimal model performance.

Step 5 - Machine Learning Model: A supervised machine learning model will be implemented to predict market values of football players. If necessary multiple models will be tested and ensembled to produce optimal learning and results.

Step 6 - Hyperparamater Fine Tuning: The Root Mean Sqaured Error (RMSE) will be the metric uses to assess accuaracy of the model, with an aim of £5m or less. Other techniques such as Variance Inflation Factor may be used in order to optimise feature selection, as well as cross-validation in order to obtain optimal model parameters.

Step 7 - User Input: This section will have the aim of creating a user input, taking the predictions from my model and comparing them to actual market values, so clubs will be able to specify and criteria of player they want to look for and are able to be pointed towards the players who's market value prediction is higher than their actual market value.

Step 8 - Presenting results: Finally a 10 minute presentation will be created, displaying the results of the project as well as delivering a live demo of the user input, to be presented to colleagues and stakeholders.
## Demographic Analysis

#### Distribution of Market Value by Age:

![Alt text](https://github.com/mattyh1010/Capstone-football-player-market-value-analysis-and-prediction/blob/main/Market%20Value%20by%20Age.png)

#### Top 10 positions by Market Value:

![Alt text](https://github.com/mattyh1010/Capstone-football-player-market-value-analysis-and-prediction/blob/main/Market%20Value%20by%20Position.png)

#### Geographical Distribution of Market Value by Nationality

![Alt text](https://github.com/mattyh1010/Capstone-football-player-market-value-analysis-and-prediction/blob/main/Market%20Value%20by%20Nationality.png)
## Machine Learning Models

#### Linear Regression Model:
- R-Squared = 0.755
- Condition. No. = 2,970 (High Multicollinearity)
- RMSE on Train data = £3.32m
- RMSE on Test data = £3.19m

#### Lasso Regression Model:
- RMSE on Train data = £3.34m
- RMSE on Test data = £3.19m

#### Ridge Regression Model:
- RMSE on Train data = £3.31m
- RMSE on Test data = £3.20m


## Chosen Model

The Ridge Regression Model was chosen as it had slightly better accuracy than the other two models and was able to better handle the high multicollinearity that was in the dataset.
## User Input

Example of user input produced, highlighting players who's market value difference is greatest comparing predicted market value to actual market value
![Alt text](https://github.com/mattyh1010/Capstone-football-player-market-value-analysis-and-prediction/blob/main/Player%20Recommender.png)
## Conclusions

Data can be used in the football player transfer markets to gain insight into which players may represent the best value for money based on their market value. With the right data to draw upon this tool could be extremely useful for clubs who do not have the same financial power as the 'bigger' clubs.
## Next Steps

A limitation of the project was not being able to find the data I wanted to in the time I had. I would like to in the future collect data that is more recent and has real world statistics, making it more useful as a real world tool.

Improving the optimisation of my model by encorporating ensembling methods
