[![Build Status](https://travis-ci.org/ices-tools-prod/icesAdvice.svg?branch=master)](https://travis-ci.org/ices-tools-prod/icesAdvice)
[![CRAN Status](http://www.r-pkg.org/badges/version/icesAdvice)](https://cran.r-project.org/package=icesAdvice)
[![CRAN Downloads](http://cranlogs.r-pkg.org/badges/grand-total/icesAdvice)](https://cran.r-project.org/package=icesAdvice)

[<img align="right" alt="ICES Logo" width="17%" height="17%" src="http://www.ices.dk/_layouts/15/1033/images/icesimg/iceslogo.png">](http://www.ices.dk/Pages/default.aspx)

icesAdvice
======

icesAdvice implements functions that are related to the advisory work of [ICES (International
Council for the Exploration of the Sea)](http://www.ices.dk/Pages/default.aspx).

icesAdvice is implemented as an [R](https://www.r-project.org) package and available on
[CRAN](https://cran.r-project.org/package=icesAdvice).

Installation
------------

icesAdvice can be installed from CRAN using the `install.packages` command:

```R
install.packages('icesAdvice')
```

Usage
-----

For a summary of the package:

```R
library(icesAdvice)
?icesAdvice
```

Calculate PA reference points:

```R
# Bpa from Blim
Bpa(Blim = 100, sigmaB = 0.15)
```

```R
# Fpa from Flim
Fpa(Flim = 0.90, sigmaF = 0.15)
```

Calculate sigma:

```R
# sigma from confidence interval
sigmaCI(lo = 100, hi = 200)
```

```R
# sigma from PA reference point
sigmaPA(lim = 100, pa = 120)
```

References
----------

ICES advisory process:

[http://ices.dk/community/advisory-process/Pages/default.aspx](http://ices.dk/community/advisory-process/Pages/default.aspx).

ICES list of software applications:

[http://ices.dk/marine-data/tools/Pages/Software.aspx](http://ices.dk/marine-data/tools/Pages/Software.aspx).

Development
-----------

icesAdvice is developed openly on [GitHub](https://github.com/ices-tools-prod/icesAdvice).
Feel free to open an [issue](https://github.com/ices-tools-prod/icesAdvice/issues) there if you encounter problems or have suggestions for future versions.

The current development version can be installed using:

```R
devtools::install_github('ices-tools-prod/icesAdvice')
```