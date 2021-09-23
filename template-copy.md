Simple document
================
Huili Zheng
2021-09-21

I’m an R Markdown document!

# Section 1

Here’s a **code chunk** that samples from a *normal distribution*:

``` r
samp = rnorm(100)
length(samp)
```

    ## [1] 100

# Section 2

I can take the mean of the sample, too! The mean is -0.0160451.

# Section 3

Here’s a **code chunk** of the learning assignment:

``` r
library(tidyverse)
set.seed(12)
plot_df <-
  tibble(
    vec_numeric = rnorm(n = 500, mean = 1),
    gr_than_0 = vec_numeric >0,
    abs_val = abs(vec_numeric)
    
  )
ggplot(plot_df, aes(x = abs_val)) + geom_histogram()
```

![](template-copy_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->
