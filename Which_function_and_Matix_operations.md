Version, platform and OS of my system
=====================================

    sessionInfo()

    ## R version 3.5.1 (2018-07-02)
    ## Platform: x86_64-w64-mingw32/x64 (64-bit)
    ## Running under: Windows 10 x64 (build 17134)
    ## 
    ## Matrix products: default
    ## 
    ## locale:
    ## [1] LC_COLLATE=English_United States.1252 
    ## [2] LC_CTYPE=English_United States.1252   
    ## [3] LC_MONETARY=English_United States.1252
    ## [4] LC_NUMERIC=C                          
    ## [5] LC_TIME=English_United States.1252    
    ## 
    ## attached base packages:
    ## [1] stats     graphics  grDevices utils     datasets  methods   base     
    ## 
    ## loaded via a namespace (and not attached):
    ##  [1] compiler_3.5.1  backports_1.1.2 magrittr_1.5    rprojroot_1.3-2
    ##  [5] tools_3.5.1     htmltools_0.3.6 yaml_2.2.0      Rcpp_0.12.18   
    ##  [9] stringi_1.1.7   rmarkdown_1.10  knitr_1.20      stringr_1.3.1  
    ## [13] digest_0.6.17   evaluate_0.11

Which function
==============

    a <- sample(1:100, 30)
    a

    ##  [1] 79 87 16 50 70 40 17 53 63 31 94  5 91 11 98 52 28 25  2 82 21 84 93
    ## [24] 12 56 89 30 41 51 27

Gives the position of element with a condition
==============================================

    which(a<50)

    ##  [1]  3  6  7 10 12 14 17 18 19 21 24 27 28 30

Direct values without positions
===============================

    a[which(a<50)]

    ##  [1] 16 40 17 31  5 11 28 25  2 21 12 30 41 27

which function with character values
====================================

    b <- c('ab','bc','cd','de','ef','fg','gh','hi','ij')

    which(b== 'de')

    ## [1] 4

    which(b!= 'hi')

    ## [1] 1 2 3 4 5 6 7 9

    d <- c('ab','bc','cd','de',NA,'fg','gh','hi','ij')
    d

    ## [1] "ab" "bc" "cd" "de" NA   "fg" "gh" "hi" "ij"

Generating Even numbers with which function
===========================================

    which((1:12)%%2 == 0)

    ## [1]  2  4  6  8 10 12

Matrix Operations
=================

    m1 <-matrix(data=1:20, nrow = 4, ncol=5, byrow = T )
    m1

    ##      [,1] [,2] [,3] [,4] [,5]
    ## [1,]    1    2    3    4    5
    ## [2,]    6    7    8    9   10
    ## [3,]   11   12   13   14   15
    ## [4,]   16   17   18   19   20

    which.max(m1)

    ## [1] 20

    which.min(m1)

    ## [1] 1

Dimensions
==========

    dim(m1)

    ## [1] 4 5

    m2 <- matrix(sample(2:30,20),nrow=4, ncol=5, byrow = T)
    m2

    ##      [,1] [,2] [,3] [,4] [,5]
    ## [1,]   29   21   13   20    9
    ## [2,]   19   16   14   24   26
    ## [3,]    5   22   28    3   25
    ## [4,]   12   17   30   18    7

Matrix Addition
===============

    m1 + m2

    ##      [,1] [,2] [,3] [,4] [,5]
    ## [1,]   30   23   16   24   14
    ## [2,]   25   23   22   33   36
    ## [3,]   16   34   41   17   40
    ## [4,]   28   34   48   37   27

    m3 <- matrix(seq(-18,20,2), nrow=5, ncol=4, byrow = F)
    m3

    ##      [,1] [,2] [,3] [,4]
    ## [1,]  -18   -8    2   12
    ## [2,]  -16   -6    4   14
    ## [3,]  -14   -4    6   16
    ## [4,]  -12   -2    8   18
    ## [5,]  -10    0   10   20

Matrix Multiplication
=====================

    Mmul1 <- m1 %*% m3
    Mmul1

    ##       [,1] [,2] [,3] [,4]
    ## [1,]  -190  -40  110  260
    ## [2,]  -540 -140  260  660
    ## [3,]  -890 -240  410 1060
    ## [4,] -1240 -340  560 1460

    Mmul2 <-m2 %*% m3
    Mmul2

    ##       [,1] [,2] [,3] [,4]
    ## [1,] -1370 -450  470 1390
    ## [2,] -1342 -352  638 1628
    ## [3,] -1120 -290  540 1370
    ## [4,] -1194 -354  486 1326
