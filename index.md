---
title       : Developing Data Products
subtitle    : Course Project
author      : Simulate Random variables and plot Histograms
job         : K Baskar
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---


## INTRODUCTION

This presentation is part of the course project for the Coursera Developing Data Products course. This has two parts. 1) create a shiny application, deploy it in Shiny server. 2) use Slidify or RStudio presenter to prepare a reproducible pitch presentation about the application. This presentation addresses the second part of the course project

The Application developed as part of the first project of this assignment can be found at: https://kcbaskar.shinyapps.io/Baskar

Source code for ui.R and server.R are found on the GitHub: https://github.com/kcbaskar/data_product


--- 
## The Inputs can be customized for the Histogram

Choose / input below parameters :


1) The data distribution type: Normal or Exponential.


2) Sample Size: Between 100 to 5000 in steps of 100


3a) For Normal Distribution, input the mean and Standard Deviation


3b) for Exponential, input the lambda


---
## Output calculations

According to the input parameter the R code populates the random variables to the vector and that Vector is then passed to the Histogram function with the other input parameters.

The R Hist function plots the Histogram.

ther is another tab, which helps the users understand this application and helps on how to use this application.

---
## Sample Histogram output


```r
randomVec <- rnorm(1000, mean = 15, sd=2)
hist(randomVec, col="blue")
```

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1-1.png) 



