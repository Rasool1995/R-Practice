---
title: "Character ops"
author: "S M Rasool"
date: "February 22, 2018"
output: md_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

## R Markdown

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:

```{r cars}
summary(cars)
```

## Including Plots

You can also embed plots, for example:

```{r pressure, echo=FALSE}
plot(pressure)
```

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.
#Creating a character vector
```{r}
names <- c('p','q','r','s','t','u')
```





#accessing a numeric vector by index 
```{r}
names[3]

names[c(3,6)]

myname <- cat(names[3],'a','s','o','o','l')
myname

```



#length
```{r}
length(names)
```




#accessing the last element
```{r}
names[length(names)]
```



#creating number sequence
```{r}

letters

letters[10:1]
```


#subsetting a vector
```{r}
new_names <- names[c(1,2,3)]  #first three
new_names

last_names <- names[(length(names) - 2) : length(names)]
last_names

```


#Vector Arithmetic
```{r}
age_after_10 <- age + 10
age_after_10
new_age<-age * 23
new_age
age <- age / 10

```


##vector + vector - Equal Size
```{r}
emp_join <- c(2010,2011,2008,2000)
emp_join
emp_leaving <- c(2017,2015,2011,2010)
emp_leaving
emp_dur <- emp_leaving - emp_join
emp_dur
```


##vector + vector - Equal Size
```{r}

emp_join1 <- c(2010,2011)
emp_join1
emp_leaving1 <- c(2017,2011,2010)
emp_leaving1
emp_dur1 <- emp_leaving1 - emp_join1
emp_dur1
```
