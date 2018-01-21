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

    ##   [1]   2 175  20 196  61  39 116 181 114  65 179 131 157 195  71 143 174
    ##  [18] 119   6 171  68 167  23  24 137  69  37 147 190  13   8 164  86 128
    ##  [35]  78  31 142  43  41   5 172  91  55  58 149  92 141  10 118   7 194
    ##  [52]  54 129  80 133  60 182  85 151 108  16 121 127  28 161  48 173 183
    ##  [69] 139 140 102  74  38  64 198  49 113 158 188  44  53  25 165 156  70
    ##  [86] 105 176 193  76 136  26 199 124  66 163 134  56  34 123 159

    #Plotting a Scatter diagram
    plot(s)

![](Hist___box_plot__files/figure-markdown_strict/unnamed-chunk-2-1.png)

    #Plotting a Histogram
    hist(s)

![](Hist___box_plot__files/figure-markdown_strict/unnamed-chunk-3-1.png)

    #Plotting a Box plot
    boxplot(s)

![](Hist___box_plot__files/figure-markdown_strict/unnamed-chunk-4-1.png)
