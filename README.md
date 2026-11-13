
<!-- README.md is generated from README.Rmd. Please edit that file -->

# assignmentB2MarinaLevy

<!-- badges: start -->

<!-- badges: end -->

The goal of assignmentB2MarinaLevy is to demonstrate Marina Levy’s
ability to create an R Package for STAT545. That being said,
assignmentB2MarinaLevy is also a usable R Package with the prebaked
(from Grace Palmer, instructor of STAT545) function
count_all_missing_by_group which counts missing values by group for a
provided data set.

## Installation

You can install the development version of assignmentB2MarinaLevy from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("UBC-STAT545-F2026/assignmentB2MarinaLevy", ref = "1.0")
```

## Example

This is a basic example showing missing data by month for the airquality
dataset:

``` r
library(assignmentB2MarinaLevy)
## basic example code for airquality data by month
count_all_missing_by_group(airquality, Month)
#> # A tibble: 5 × 6
#>   Month Ozone Solar.R  Wind  Temp   Day
#>   <int> <int>   <int> <int> <int> <int>
#> 1     5     5       4     0     0     0
#> 2     6    21       0     0     0     0
#> 3     7     5       0     0     0     0
#> 4     8     5       3     0     0     0
#> 5     9     1       0     0     0     0
```
