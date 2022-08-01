# MarchMadness
## Context
This repository contains all the code I implemented for the 2022 March Madness. An annual competition sponsored by **Kaggle** which goal is to predict the outcomes of the US men's college basketball tournament. In order to do so, Kaggle provides us historical NCAA games data.

The challenge is divided into 2 parts :
 - Train a model to predict tourney results on the previous years (2016-2021).
 - Predict 2022 results

## First Part

 - After Selection Sunday, **68 teams** have been selected.

 - Results are expected on the last 5 editions : **2016, 2017, 2018, 2019 & 2021**

 - We have to predict all 67*68/2 = **2278** possible combinations per year.

The file to be submitted consists of a DataFrame with :
 - the match ID consisting of the year and team ids (year_id1_id2) 
 - the probability that team Id1 wins.

 - A total of 5*2278 = 11 390 matches
 - The score is computed with the Log Loss :

![](Images/Capture d’écran 2022-08-01 à 22.44.52.png "LogLoss")
