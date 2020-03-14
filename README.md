## Repository of R packages by [Petr Bouchal](https://petrbouchal.github.io)

Install packages from this repository like so (example for the `pragr` package):

``` r 
install.packages("pragr", repos = "https://petrbouchal.github.io/drat/")
```

Or, to gain more direct access to this package repository, put this in your .Rprofile:

```r
local({r <- getOption("repos")
# add drat repo
r["petrbouchal"] <- "petrbouchal.github.io/drat"
options(repos=r)})
```

...then you will be able to do just

``` r
install.packages("pragr")
```

even though the `pragr` package is not on CRAN.

This may be preferable to using e.g. `remotes::install_github("petrbouchal/<package>")` since you

- always get a release, rather than the latest snapshot, which may be broken.
- get a binary package if available
- get a package with the vignettes built by default

Currently the repository contains the following packages:

- [czso](https://github.com/petrbouchal/czso) for accessing open data from the Czech Statistical Office 
- [pragr](https://github.com/petrbouchal/pragr) for visualising data about Prague
- [statnipokladna](https://github.com/petrbouchal/statnipokladna) for Czech public finance data
- [ptrr](https://github.com/petrbouchal/ptrr), a collection of personal utilities

Source code for all the packages is hosted on [Github](https://github.com/petrbouchal).

The repository has been created using the `drat` package by @eddelbuettel; see more at <http://dirk.eddelbuettel.com/code/drat.html>

More on
