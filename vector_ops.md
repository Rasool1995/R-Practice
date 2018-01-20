R Markdown
----------

Creating a numeric vector
=========================

    marks <- c(33,56,43,87,96)
    marks

    ## [1] 33 56 43 87 96

accessing a numeric vector by index
===================================

    marks[1]

    ## [1] 33

    marks[c(2,5)]

    ## [1] 56 96

    marks[-c(3,5)]

    ## [1] 33 56 87

Plot
----

    plot(marks)

![](vector_ops_files/figure-markdown_strict/unnamed-chunk-3-1.png)

Replacing elements by index
===========================

    marks[3] <- 66
    marks

    ## [1] 33 56 66 87 96

length
======

length(marks)

accessing the last element
==========================

marks\[length(marks)\]

creating number sequence
========================

10: 6

90: 99

subsetting a vector
===================

sub\_marks &lt;- marks\[5:2\] sub\_marks

length(marks) last\_3\_marks &lt;-
marks\[c(length(marks)-2:length(marks))\] last\_3\_marks

first three
===========

First\_3\_marks &lt;- marks\[1:3\] First\_3\_marks

Vector Arithmetic
=================

marks\_with\_practicals &lt;- marks + 50 marks\_with\_practicals

percentage\_marks&lt;-
(marks\[1\]+marks\[2\]+marks\[3\]+marks\[4\]+marks\[5\])/500 \*100
percentage\_marks

vector + vector - Equal Size
----------------------------

std\_paid\_fee &lt;- c(20, 40, 30, 55) std\_paid\_fee std\_total\_fee
&lt;- c(100,150,400,60) std\_total\_fee remaining\_fee &lt;-
std\_total\_fee - std\_paid\_fee

vector + vector - Equal Size
----------------------------

std\_join\_date &lt;- c(2012,2011, 2000) std\_join\_date std\_comp\_date
&lt;- c(2017,2018) std\_comp\_date duration\_student &lt;-
std\_join\_date + std\_comp\_date

It will show warning message about length
=========================================
