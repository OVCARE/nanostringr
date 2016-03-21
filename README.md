nanostringr
===========

An R Package for quality assurance checking, normalization and batch effects adjustments of NanoString data suitable for single sample processing. This is the companion R package for the paper published in XXX.

Installation
------------

To install this package, use devtools:

``` r
#devtools::install_github("OVCARE/nanostringr")
```

Dependencies
------------

Please note that the package CHL26predictor (<https://github.com/tinyheero/CHL26predictor>) is needed to run the Hodgkin Lymphoma predictive model.

Overview
--------

To see the full list of exported functions:

``` r
library(nanostringr)
ls("package:nanostringr")
#> [1] "expQC"        "HKnorm"       "hld.r"        "hlo.r"       
#> [5] "NanoStringQC" "ovc.r"        "ovd.r"        "ovo.r"       
#> [9] "refMethod"
```

A quick overview of the key functions:

-   NanoStringQC: Computes quality assurance metrics.
-   HKnorm: Performs log (base 2) transformation and normalization to Housekeeping Genes
-   refMethod: Performs batch effect correction using the reference-based strategie
