# Predicting the Improvement of La Liga players

## Introduction


__Background__

The _Campeonato Nacional de Liga de Primera División_, commonly known as _La Liga_ is the men's top professional football division of the Spanish football league system. _La Liga_ is a famous football league in the world with millions of fans worldwide. How players on a team perform is the most important factor that determines which team wins the championship. Players’ pay are largely based on their past performances. However, player performance change from season to season. Each year there are a number of players who improve dramatically over last year. Those players bring a lot of value, both competitively and economically, to the teams they belong to. Therefore, it is advantageous for teams to accurately predict whether and how much a player will improve in the next season. For example, this information can be used to target players to acquire in trades or signings.

__Problem__

Data that might contribute to determining player improvement might include his performance last season, his position, and metrics that describe what kind of player he is. This project aims to predict whether or not a player will improve the next season based on these data.

__Interest__

_La Liga_ teams would be very interested in accurate prediction of player improvement, for competitive advantage and business values. Others who are interested in _La Liga_ such as fans and fantasy football players may also be interested.

## Data 

__Data sources__

Most player stats, position, and other data can be found in this Kaggle dataset https://www.kaggle.com/alvarob96/laliga_2018-19_season_player_stats

__Data cleaning & Feature Selection__

Non-relevant data for this purpose has been removed from this dataset, therefore only the following parameters have been selected:

* Minutes played
* Goals scored
* Passes
* Interceptions
* Recoveries

## Exploratory Data Analysis

Player improvement for the next season was not a feature in the dataset, and had to be calculated. I chose to do different calculations depending on player position:

* Forward: Minutes Played>=500 & Goals scored>=3 --> He/They will improve next season
* Midfielder: Minutes Played>=500 & Passes>=350 --> He will improve next season
* Defender: Interceptions>=25 & Recoveries>=50 ---> He will improve next season
* Goalkeeper: Recoveries>=150 ---> He will improve next season

## Results
You discuss the results.

## Discussion & Conclusion
You discuss any observations you noted and any recommendations you can make based on the results.
Conclusion section where you conclude the report.

