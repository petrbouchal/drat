## Repository of R packages by [Petr Bouchal](https://petrbouchal.github.io)

Install packages from this repository like so (example for the `pragr` package):

``` r 
install.packages("pragr", repos = "https://petrbouchal.github.io/drat/")
```

Or, to set this permanently and without the `drat` dependency, put this in your .Rprofile:

```r
local({r <- getOption("repos")
# add drat repo
r["petrbouchal"] <- "petrbouchal.github.io/drat"
options(repos=r)})
```

This may be preferable to using `remotes::install_github("petrbouchal/pragr")` since you

- always get a release, rather than the latest snapshot, which may be broken.
- get a binary package if available
- get a package with the vignettes built by default

If you'd like to add this repository to the list of places where R looks for packages, run

``` r
drat::addRepo("petrbouchal")
```

...then you will be able to do just

``` r
install.packages("pragr")
```

even though the `pragr` package is not on CRAN.


Currently the repository contains the following packages:

- [czso](https://github.com/petrbouchal/czso) for accessing open data from the Czech Statistical Office 
- [pragr](https://github.com/petrbouchal/pragr) for visualising data about Prague
- [statnipokladna](https://github.com/petrbouchal/statnipokladna) for Czech public finance data

Source code for all the packages is hosted on [github](https://github.com/petrbouchal).

The repository has been created using the `drat` package by @eddelbuettel; see more at <http://dirk.eddelbuettel.com/code/drat.html>

More on

- [twitter](https://twitter.com/petrbouchal)
- [linkedin](https://linkedin.com/in/petrbouchal)
