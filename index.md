---
title       : Amount accumulated based on Compound Interest
subtitle    : Description
author      : Surya
job         : Engineer
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction

This Shiny Application is used to find the Compound interest and finally the total amount accumulated for a given principal, interest rate, no of times compounded per year and the time in years

--- .class #id 

## Inputs to the Application

User needs to enter the following Inputs :

1) Principal, P

2) Rate of Interest, r

3) No of time compounded per year, n

4) Time period in years, t

--- .class #id 

## Formulation 

Following is the textbook formulation for Compound interest and Amount accumulated 

Compound Interest = P * (1 + r/ n )^(r*t) - P

Amount Accumulated = P * (1 + r/ n )^(r*t)

--- .class #id 

## Example 


```r
P = 1e+05
r = 0.5
n = 2
t = 1
Compound_interest = P * (1 + r/n)^(r * t) - P
Amount_accumulated = P * (1 + r/n)^(r * t)
print(paste("Compound Interest is ", as.integer(Compound_interest), sep = "Rs."))
```

```
## [1] "Compound Interest is Rs.11803"
```

```r
print(paste("Amount accumulated is  ", as.integer(Amount_accumulated), sep = "Rs."))
```

```
## [1] "Amount accumulated is  Rs.111803"
```




