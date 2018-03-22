Project 1
=========

##Setup

Loading necessary packages to start the work.

```r
library(ggplot2)
library(dplyr)
library(lubridate)
library(knitr)
setwd("C:\\Users\\barca\\Desktop\\DATA SCIENCE\\Reproducible Research week 2") # Change to your WD if necessary. 
```

Loading and doing some transformations with data.


```r
stepsData <- tbl_df(read.csv("activity.csv", header = T, na.strings = "NA", col.names = c("Steps", "Date", "Interval")))
stepsData$Date <- ymd(stepsData$Date)
```
##Part 1 - Total steps
Calculating total number of steps by days and building a histogram using ggplot2 package.






















