# Indian-premier-league-IPL-First-Innings-Score-Prediction
![FISP](readme-resources/first-innings-banner.png)
![Python](https://img.shields.io/badge/Python-3.6-brightgreen.svg) ![sklearn](https://img.shields.io/badge/Library-sklearn-orange.svg)

## Project Overview
• Created a model that predicts the score (in terms of range) of IPL matches<br/>
• Optimized Multiple-Linear, Decision Tree, Random Forest, and AdaBoost regression models using GridsearchCV

## How will this project help?
• This project is for the fantasy cricket fans out there, helping them to earn extra fantasy points for Dream11 IPL 2020

## Resources Used
• Packages: pandas, numpy, sklearn, matplotlib, seaborn<br/>
• 617 IPL matches -> data/ipl.csv

## Each dataset consists of the following columns:

* mid -> Each match is given a unique number
* date -> When the match happened
* venue -> Stadium where match is being played
* bat_team -> Batting team name
* bowl_team -> Bowling team name
* batsman -> Batsman name who faced that ball
* bowler -> Bowler who bowled that ball
* runs -> Total runs scored by team at that instance
* wickets -> Total wickets fallen at that instance
* overs -> Total overs bowled at that instance
* runs_last_5 -> Total runs scored in last 5 overs
* wickets_last_5 -> Total wickets that fell in last 5 overs
* striker -> max(runs scored by striker, runs scored by non-striker)
* non-striker -> min(runs scored by striker, runs scored by non-striker)
* total -> Total runs scored by batting team after first innings

## Data Cleaning and Preprocessing
• **Removing unwanted columns**<br/>
• **Keeping only consistent teams**<br/>
![ct](readme-resources/consistent_teams.PNG)<br/>
• **Removing the first 5 overs data in every match**<br/>
• **Converting the column 'date' from string into datetime object**<br/>
• **Handling categorical features**

## Model Building and Evaluation
Evaluation metric: Root Mean Squared Error (RMSE)<br/>
• Multiple Linear Regression - 15.843 <br/>
• Decision Tree - 23.044<br/>
• Random Forest - 18.171<br/>
• **Adaptive Boosting (AdaBoost) - 15.798**

## Model Prediction
![pred](readme-resources/prediction.PNG)<br/>

## Future Scope
• Add columns in dataset of top batsmen and bowlers of all the teams.<br/>
• Add columns that consists of striker and non-striker's strike rates.<br/>
• Implement this problem statement using Artificial Neural Network (ANN).<br/>
