---
title       : Shiny App and Reproducible Pitch
subtitle    : Cours Project - Data Development Product
author      : Dmitry Ermakov
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---
## About GDP2013

  This app GDP2013 made by Dmitry Ermakov as part of Course Project: *"Shiny Application and Reproducible Pitch"*. It helps to review the Gross Domestic Product 2013 by countries. 
###  Files
* README.md  - This text
* cleaning.R - Data preparation process.
* ui.R      - User-interface script
* server.R   - Server script
* df.RData - Data set

--- .class #id 

## Data description
The data donwloaded from **THE WORLD BANK** and prepared in CLEANING.R module.
http://api.worldbank.org/v2/en/indicator/ny.gdp.mktp.cd?downloadformat=csv

The final structure of data:

```
##          Country     usd rank
## 1 European Union 17958.1    1
## 2  United States 16768.1    2
## 3          China  9240.3    3
## 4          Japan  4919.6    4
## 5        Germany  3730.3    5
## 6     Arab World  2853.1    6
```

```
## [1] 156   3
```


--- .class #id 

## How to use
### MAP
The tab MAP shows GDP on geografical map. Selecet the region on side panel Choose region and choose rank of countries on GDP Rank. Move the mouse coursor to the country on the map and you will see the name and GDP in billions US dollars
### PLOT
The tab PLOT shows plot of GDP by countries. Choose rank of countries on GDP Rank on the side panel.
### DATA
The tab DATA shows GDP data table. Choose rank of countries on GDP Rank on the side panel and you will see result in the table. You can use 'search:' and switch pages in the table.

--- .class #id 

## Hosting for GDP 2013
The app hosted on ShinyApps server.
http://dimakrat.shinyapps.io/GDP2013

![](http://github.com/dimakrat/GDP2013/raw/master/gdpMap.png)

