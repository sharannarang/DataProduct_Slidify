---
title       : Football Statistics 
subtitle    : Simplifying the football world!
author      : Sharan Narang
job         : Developing Data Products Project
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction

* Football (Soccer) is the most popular sport in the world played in over 200 countries. 

* European club football has a collection of the leading football stars from all over the world. Many teams are composed of players with varying nationalities. 

* The style of football can vary drastically from fast paced English Premier League to highly tactical Spanish La Liga.

* As a consequence, some of the most intriguing & exciting football is played across various European Leagues.

---

## Why do we need more statistics in football?
* An average football match doesn't contain a lot of goals. We compute the average number of goals scored over 380 English Premier League games using the EPL results data. 


```r
# Contains results of every premier league game from 2013-2014 season
epl.data <- read.csv("epl.csv") 

# Compute the average goals scored per game
sum(epl.data$FTHG + epl.data$FTAG)/nrow(epl.data) 
```

```
## [1] 2.768
```

* In order to analyse the sport, it is important to look beyond just the goals. 

* As important as are, more statistics are required to fully understand the game.

---

## Statistics

* To help understand some details of the sport, we have compiled per team statistics of the following parameters:
    * Total Goals
    * Total Points
    * Total Goals Conceeded
    * Home Goals
    * Away Goals
    * Yellow Cards
    * Red Cards
    * Shots on Target

---

## Usage

* We have analysed results over the last 3 years and compiled statistics for the following leagues:
    * English Premier League
    * Spanish La Liga
    * German Bundesliga
    * Italian Serie A

* Using the inputs on the webpage, a chart is generated depicting the statistic for each team for a selected season.

* To use the website, please visit: https://sharan.shinyapps.io/Project/

* Have fun!


