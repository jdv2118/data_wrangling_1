Data Import
================

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.2 ──
    ## ✔ ggplot2 3.3.6      ✔ purrr   0.3.4 
    ## ✔ tibble  3.1.8      ✔ dplyr   1.0.10
    ## ✔ tidyr   1.2.0      ✔ stringr 1.4.1 
    ## ✔ readr   2.1.2      ✔ forcats 0.5.2 
    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()

## Data Import: CSVs

Let’s import data using the `readr` package.

``` r
read_csv("data/FAS_litters.csv")
```

    ## Rows: 49 Columns: 8
    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr (2): Group, Litter Number
    ## dbl (6): GD0 weight, GD18 weight, GD of Birth, Pups born alive, Pups dead @ ...
    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

    ## # A tibble: 49 × 8
    ##    Group `Litter Number` `GD0 weight` GD18 wei…¹ GD of…² Pups …³ Pups …⁴ Pups …⁵
    ##    <chr> <chr>                  <dbl>      <dbl>   <dbl>   <dbl>   <dbl>   <dbl>
    ##  1 Con7  #85                     19.7       34.7      20       3       4       3
    ##  2 Con7  #1/2/95/2               27         42        19       8       0       7
    ##  3 Con7  #5/5/3/83/3-3           26         41.4      19       6       0       5
    ##  4 Con7  #5/4/2/95/2             28.5       44.1      19       5       1       4
    ##  5 Con7  #4/2/95/3-3             NA         NA        20       6       0       6
    ##  6 Con7  #2/2/95/3-2             NA         NA        20       6       0       4
    ##  7 Con7  #1/5/3/83/3-3/2         NA         NA        20       9       0       9
    ##  8 Con8  #3/83/3-3               NA         NA        20       9       1       8
    ##  9 Con8  #2/95/3                 NA         NA        20       8       0       8
    ## 10 Con8  #3/5/2/2/95             28.5       NA        20       8       0       8
    ## # … with 39 more rows, and abbreviated variable names ¹​`GD18 weight`,
    ## #   ²​`GD of Birth`, ³​`Pups born alive`, ⁴​`Pups dead @ birth`, ⁵​`Pups survive`
