
<!-- README.md is generated from README.Rmd. Please edit that file -->

# regexcite

<!-- badges: start -->

<!-- badges: end -->

The goal of regexcite is to make regular expressions more exciting! It
provides convenience functions to make some common tasks with string
manipulation and regular expressions a bit easier.

## Installation

You can install the development version of regexcite from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("nshack99/regexcite")
```

## Example

A common task when dealing with strings is splitting a single string
into many parts:

``` r
library(regexcite)

x <- "alfa,bravo,charlie,delta"
str_split_one(x, pattern = ",")
#> [1] "alfa"    "bravo"   "charlie" "delta"
```

You can also use the `n` argument to limit the number of splits:

``` r
str_split_one(x, pattern = ",", n = 2)
#> [1] "alfa"                "bravo,charlie,delta"
```
