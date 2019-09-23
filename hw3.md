---
title: "Homework 3"
author: 'Cheetah'
date: "9/19/2019"
output: 
  html_document:
    keep_md: yes
---



# Introduction

>America does a poor job tracking and accounting for its unsolved homicides. 
Every year, at least 5,000 killers get away with murder. The rate at which 
police clear homicides through arrest has declined over the years until, today, 
about a third go unsolved.
<br/><br/>
The Murder Accountability Project is a nonprofit group organized in 2015 and 
dedicated to educate Americans on the importance of accurately accounting for 
unsolved homicides within the United States.

<img src="map.png" width="600" height="200">

# Packages


```r
library(tidyverse)
```

# Data


```r
murder <- read_csv("https://www.dropbox.com/s/wzp6o78lcosp3ux/map.csv?dl=1")
names(murder) <- tolower(names(murder))
```

# Tasks

## Task 1

#### 1.How many distinct counties in North Carolina had a recorded homicide in 2017?

```r
murder %>%
  filter(state=='North Carolina', year==2017) %>%
 # select(cntyfips) %>%
  summarise(n_distinct(cntyfips))
```

```
# A tibble: 1 x 1
  `n_distinct(cntyfips)`
                   <int>
1                     73
```
#### 2.Which year and month combinations had the three most homicides in North Carolina from 2013 to 2017?

```r
murder %>%
  filter(state=='North Carolina', year>=2013 & year<=2017) %>%
  group_by(year, month) %>%
  summarize(count = n()) %>%
  arrange(desc(count)) %>%
  head(3)
```

```
# A tibble: 3 x 3
# Groups:   year [2]
   year month  count
  <dbl> <chr>  <int>
1  2017 August    70
2  2016 March     64
3  2017 April     63
```

```r
  # slice(1:3)
```

#### 3.What were the top three states that had the most homicides by "Murder and non-negligent manslaughter" that were solved and crossed racial lines, i.e., where the offender and victim were of different race? Include the counts in your answer.


## Task 2
