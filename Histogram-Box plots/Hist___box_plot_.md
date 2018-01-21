R Markdown
----------

This is an R Markdown document. Markdown is a simple formatting syntax
for authoring HTML, PDF, and MS Word documents. For more details on
using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that
includes both content as well as the output of any embedded R code
chunks within the document. You can embed an R code chunk like this:

    summary(cars)

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

Including Plots
---------------

You can also embed plots, for example:

![](Hist___box_plot__files/figure-markdown_strict/pressure-1.png)

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.

    #Creating a sample Vector
    s  <- sample(1:200,100)
    s

    ##   [1] 135  88  41 182 163  74  42  40  35 121 130 159  79  16 128   6  66
    ##  [18]  33  57  52 199 166 106 148  18 101  31 124  30 152 198 196  23  46
    ##  [35] 156 102  24 167   5 195  56  91  48   9  93   8 165  26  27  36 117
    ##  [52] 125 155 132 149 153  61  96  49  77 139 145 178  10  59  98 186  37
    ##  [69] 174 107 189 127 119 200  39   1  60  94 120 134 162  65  32  80  71
    ##  [86]  86 179  67 183   4 185  92 154  34 151  45 193 112 188 131

Plotting a Scatter diagram
==========================

plot(s)

Plotting a Histogram
====================

hist(s)

Plotting a Box plot
===================

boxplot(s)
