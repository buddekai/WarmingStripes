README
================

climateStripes
--------------

R package to create diagrams that show the impact of climate change. It started with an R function to plot Warming Stripes which were inspired by Ed Hawkins. The R package can now fetch data from Deutscher Wetterdienst (DWD) and plot:

-   [Warming Stripes](#warming-stripes) (annual deviation from the average temperature in the years 1961-1990 as colored bars)
-   [Precipitation Stripes](#precipitation-stripes) (annual deviation from the average total precipitation in the years 1961-1990 as colored bars)

(Most recent additions may be found in the develop-branch.)

### How to install the package and use it

In order to create all possible plots for the DWD station in Rostock, one needs to download the package and execute the following lines of code in R:

``` r
library(devtools)
install()
require("climateStripes")
climateStripes(city.name = "rostock")
```

### Examples: How to create different climate plots

#### Warming Stripes

``` r
library(devtools)
install()
require("climateStripes")
climateStripes(city.name = "rostock", plot.what = "warmingstripes")
```

``` r
knitr::include_graphics("man/figures/WarmingStripes.png")
```

<img src="man/figures/WarmingStripes.png" width="100%" style="display: block; margin: auto;" />

#### Precipitation Stripes

``` r
library(devtools)
install()
require("climateStripes")
climateStripes(city.name = "rostock", plot.what = "precipitationstripes")
```

``` r
knitr::include_graphics("man/figures/PrecipitationStripes.png")
```

<img src="man/figures/PrecipitationStripes.png" width="100%" style="display: block; margin: auto;" />
