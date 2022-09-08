--- 
title: "Environmental Informatics Using Research Infrastructures and their Data"
author: "Dr. Katharyn Duffy, Dr. Ben Ruddell"
#date: "2020 Edition"
cover-image: "/Users/kdw223/Research/katharynduffy.github.io/images/EcoInfo4.png"
site: bookdown::bookdown_site
output: bookdown::gitbook
documentclass: book
github-repo: 'katharynduffy/katharynduffy.github.io'
description: "Course text for NAU INF 550"
always_allow_html: true
---

# Preface {-}

Placeholder


## Acknowledgements {-}
### Key Contributors {-}

<!--chapter:end:index.Rmd-->


# Pre-Course Setup: EcoInformatics Tools {-}

Placeholder


## Pre-Course Skills & Setup
### Installing or Updating R
### Windows R/RStudio Setup
### Mac R/RStudio Setup
## Linux R/RStudio Setup
### Install basic packages for this course
## Installing and Setting up Git & Github on Your Machine
## Installing Atom
## Linking RStudio to Git
## How we will be Conducting this Course
## Exercises:
## The Framework of this Course
## Final Course Project: Proposed Derived Data Product

<!--chapter:end:01_Pre-Course_Skills.Rmd-->


# Introduction to NEON & its Data

Placeholder


## Learning Objectives
## The NEON Project Mission & Design
## The Science and Design of NEON
## NEON's Spatial Design
### NEON Samples All 20 Eco-Regions
## How NEON Collects Data
### Specimens & Samples
### Airborne Remote Sensing
## Accessing NEON Data
### Pathways to access NEON Data
## Hands on: Accessing NEON Data & User Tokens
### Via the NEON API, with your User Token
### Objectives
### Things You'll Need To Complete This Tutorial
### Install R Packages
## Additional Resources
### Get a NEON API Token
### Use the API token in neonUtilities
### Token management for open code
#### Option 1: Save token in a local file
#### Option 2: Save your toekn to your R environment
## Hands on: NEON TOS Data
### Pull in Tree Data from NEON's TOS and investigate relationships
## Intro to NEON Exercises Part 1
### Exercise 2.1: Computational
#### Sign up for and Use an NEON API Token:
#### Further Investigation of NEON TOS Vegetation Structure Data
## Hands on: Pulling NEON Data via the API
### Objectives
### Things You'll Need To Complete This Section
#### Install R Packages
#### Additional Resources
## What is an API?
### Anatomy of an API call
#### Base URL:
#### Endpoints:
### Targets:
### Observational data (OS)
### Instrumentation data (IS)
### Remote sensing data (AOP)
### Geolocation data
#### Instrumentation data (both aquatic and terrestrial)
#### Observational data - Terrestrial
### Querying a single named location
### Taxonomy
## Stacking NEON data
## Intro to NEON Exercises Part 2
### Exercise 2.2: Written questions
### Exercise 2.3: NEON Coding Lab
### Exercise 2.4: Intro to NEON Culmination Activity

<!--chapter:end:02_Introduction_to_NEON.Rmd-->


# Introduction to USA-NPN & its Data

Placeholder


## USA-NPN Learning Objectives
## USA-NPN Project Mission & Design:
## Vision & Mission
### Relevant documents & background information:
## USA-NPN’s Spatial design:
## Types of USA-NPN Data:
### Observational
### Status & Intensity Data
### Gridded Raster Data
### Pheno-Forecasts
## How to Access USA-NPN Data:
### The USA-NPN Landing page
### APIs
### Rnpn package
### Phenology Observation Portal (for observational data)
### Geospatial Request Builder (for raster data and image files)
### Visualization Tool
## USA-NPN Written Questions
## Hands on: Accessing USA-NPN Data via rNPN
### Introduction
### Accessing USA-NPN Observational Data
#### Basic format for for Observational data calls
#### Required Parameters
#### Find stations at which a species has been observed
### Status and Intensity Data
### Individual Phenometrics
### Site Phenometrics
### Magnitude Phenometrics
### USA-NPN Geospatial Data
## Accumulated Growing Degree Day Products
## Extended Spring Indices
### Other Layers
## Putting it all together:
## Combine Point and Raster Data
### Step 1: Get the data
### Step 2: Preparing the data
### Step 3: Define style options and create graph
## Live Demo Code with Lee Marsh of USA-NPN
### Basic Utility Functions
### Download Observational Data
### Magnitude Data
### Downloading Geospatial Data
### Putting it together
### Other Data Sources, e.g. Daymet, MODIS
## USA-NPN Coding Lab
## NEON TOS Phenology Data Lecture
## Understanding Observation Biases and Censoring in Citizen Science Data
### Many existing modeling approaches fail in one (or both) regards.
### Censoring
## So then how can we model censored data?
## Intro to USA-NPN Culmination Activity

<!--chapter:end:03-USA-NPN.Rmd-->


# PhenoCam: Digital Repeat Photography Networks & Methods

Placeholder


## Digital Repeat Photography Networks Learning Objectives
## The PhenoCam Network Mission & Design
### Relevant documents & background information:
## PhenoCam’s Spatial design:
### PhenoCam as a Near Surface Remote Sensing Technique
### How PhenoCams Pull Data
### Leveraging camera near-infrared (NIR) capabilities
## Digital Repeat Photography Written Questions
## Introduction to Digital Repeat Photography Methods
## Pulling Data via the *phenocamapi* Package
## Exploring PhenoCam metadata
### Remove null values
### Filtering using attributes
## Download midday images
### Download midday images for a given time range
## Detecting Foggy Images using the 'hazer' R Package
#### Read & Plot an Image
#### Histogram of RGB channels
#### Brightness
#### Darkness
#### Contrast
#### Image fogginess & haziness
#### Process sets of images
## Extracting Timeseries from Images using the xROI R Package
### xROI Design
### Install xROI
### Launch xROI
### End xROI
### Use xROI
## Documentation and Citation
### Challenge: Use xROI
## Hands on: Digital Repeat Photography Computational
### PhenoCam time series
### Obtain ROIs
### Download time series
### Threshold values
### Comparing phenology across vegetation types
### In Class Hands-on Coding: Comparing phenology of the same plant function type (PFT) across climate space
## Digital Repeat Photography Coding Lab
### Quantifying haze and redness to evaluate California wildfires
## PhenoCam Culmination Activity

<!--chapter:end:05-PhenoCam.Rmd-->


# Flux Measurements & Inter-Operability


>Estimated Time: 3 hours


<div id="ds-challenge" markdown="1">


<div id="ds-challenge" markdown="1">
**Course participants**: As you review this information, please
consider the final course project
that you will work on at the over this semester. At the end of this section, you will
document an initial research question or idea and associated data needed to
address that question, that you may want to explore while pursuing this course.


## Learning Objectives

At the end of this activity, you will be able to:

* Define the eddy covariance method

* Articulate various carbon storage and flux terms

* Understand the structure of bundled eddy covariance data

* Be able to process NEON flux data such that it is comparable with AmeriFlux


## Eddy Co_variance Data: What does it actually measure?
 
<iframe width="560" height="315" src="https://www.youtube.com/embed/CR4Anc8Mkas" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Example Eddy Site

<iframe width="560" height="315" src="https://www.youtube.com/embed/XrxZy7Dp4ko" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## QA/QC Flags





## Examples of Other Flux Networks: AMERIFLUX & FLUXNET

AmeriFlux is a [network of PI-managed sites]() measuring ecosystem CO2, water, and energy fluxes in [North, Central and South America](https://ameriflux.lbl.gov/sites/site-search/#filter-type=all&has-data=All&site_id=). It was established to connect research on field sites representing major climate and ecological biomes, including tundra, grasslands, savanna, crops, and conifer, deciduous, and tropical forests. As a grassroots, investigator-driven network, the AmeriFlux community has tailored instrumentation to suit each unique ecosystem. This “coalition of the willing” is diverse in its interests, use of technologies and collaborative approaches. As a result, the AmeriFlux Network continually pioneers new ground.

The network was launched in 1996, after an international workshop on flux measurements in La Thuile, Italy, in 1995, where some of the first year-long flux measurements were presented. Early support for the network came from many sources, including the U.S. Department of Energy’s Terrestrial Carbon Program, the DOE’s National Institute of Global Environmental Change (NIGEC), NASA, NOAA and the US Forest Service. The network grew from about 15 sites in 1997 to more than 110 active sites registered today. Sixty-one other sites, now inactive, have flux data stored in the network’s database. In 2012, the U.S. DOE established the AmeriFlux Management Project (AMP) at Lawrence Berkeley National Laboratory (LBNL) to support the broad AmeriFlux community and the AmeriFlux sites.

[View the AMERIFLUX Network-at-a-Glance](https://ameriflux.lbl.gov/about/network-at-a-glance/)

AmeriFlux is now one of the DOE Office of Biological and Environmental Research’s (BER) best-known and most highly regarded brands in climate and ecological research. AmeriFlux datasets, and the understanding derived from them, provide crucial linkages between terrestrial ecosystem processes and climate-relevant responses at landscape, regional, and continental scales.

## The Power of Networked Ecology: Bridging to AMERIFLUX and Beyond

Given that [AmeriFlux](https://ameriflux.lbl.gov/) has been collecting and coordinating eddy covariance data across the Americas since 1996. The network provides a common platform for data sharing and collaboration for organizations and individual private investigators collecting flux tower data. There are now >470 registered flux tower sites in North, Central, and South America in the AmeriFlux network, many operated by individual researchers or universities. The towers collect eddy covariance data across a broad range of climate zones and ecosystem types, from Chile to Alaska and everywhere in between.

Now, data from the NEON project is available through the AmeriFlux data portal. The NEON team has formatted data from the NEON flux towers to make it fully compatible with AmeriFlux data. This allows researchers to view, download and analyze data from the NEON flux towers alongside data from all of the other flux towers in the AmeriFlux network.

With 47 flux towers at terrestrial field sites across the U.S., the NEON program is now the largest single contributor of flux tower data to the AmeriFlux network. NEON field sites are located in 20 ecoclimatic zones across the U.S., representing many distinct ecosystems. Eddy covariance data will be served using the same methods at each site for the entire 30-year life of the Observatory, allowing for unprecedented comparability across both time and space.

## Hands On: Introduction to working with NEON eddy flux data

### Setup

Start by installing and loading packages and setting options. 
To work with the NEON flux data, we need the `rhdf5` package, 
which is hosted on Bioconductor, and requires a different 
installation process than CRAN packages:


```
install.packages('BiocManager')
BiocManager::install('rhdf5')
```


```r
options(stringsAsFactors=F)

library(neonUtilities)
```

Use the `zipsByProduct()` function from the `neonUtilities` package to 
download flux data from two sites and two months. The transformations 
and functions below will work on any time range and site(s), but two 
sites and two months allows us to see all the available functionality 
while minimizing download size.

Inputs to the `zipsByProduct()` function:

* `dpID`: DP4.00200.001, the bundled eddy covariance product
* `package`: basic (the expanded package is not covered in this tutorial)
* `site`: NIWO = Niwot Ridge and HARV = Harvard Forest
* `startdate`: 2018-06 (both dates are inclusive)
* `enddate`: 2018-07 (both dates are inclusive)
* `savepath`: modify this to something logical on your machine
* `check.size`: T if you want to see file size before downloading, otherwise F

The download may take a while, especially if you're on a slow network.



```r
zipsByProduct(dpID="DP4.00200.001", package="basic", 
              site=c("NIWO", "HARV"), 
              startdate="2018-06", enddate="2018-07",
              savepath="./data", 
              check.size=F)
```

```
## Finding available files
## 
  |                                                                            
  |                                                                      |   0%
  |                                                                            
  |==================                                                    |  25%
  |                                                                            
  |===================================                                   |  50%
  |                                                                            
  |====================================================                  |  75%
  |                                                                            
  |======================================================================| 100%
## 
## Downloading files totaling approximately 345.260177 MB
```

```
## ./data/filesToStack00200 already exists. Download will proceed, but check for duplicate files.
```

```
## Downloading 4 files
## 
  |                                                                            
  |                                                                      |   0%
  |                                                                            
  |=======================                                               |  33%
## NEON.D01.HARV.DP4.00200.001.2018-06.basic.20220120T173946Z.RELEASE-2022.zip could not be downloaded. Re-attempting.
## 
  |                                                                            
  |===============================================                       |  67%
## NEON.D01.HARV.DP4.00200.001.2018-07.basic.20220120T173946Z.RELEASE-2022.zip could not be downloaded. Re-attempting.
## 
  |                                                                            
  |======================================================================| 100%
## NEON.D13.NIWO.DP4.00200.001.2018-07.basic.20220120T173946Z.RELEASE-2022.zip could not be downloaded. Re-attempting.
## 
## 4 files successfully downloaded to ./data/filesToStack00200
```



### Data Levels

There are five levels of data contained in the eddy flux bundle. For full 
details, refer to the <a href="http://data.neonscience.org/api/v0/documents/NEON.DOC.004571vA" target="_blank">NEON algorithm document</a>.

Briefly, the data levels are:

* Level 0' (dp0p): Calibrated raw observations
* Level 1 (dp01): Time-aggregated observations, e.g. 30-minute mean gas concentrations
* Level 2 (dp02): Time-interpolated data, e.g. rate of change of a gas concentration
* Level 3 (dp03): Spatially interpolated data, i.e. vertical profiles
* Level 4 (dp04): Fluxes

The dp0p data are available in the expanded data package and are beyond 
the scope of this tutorial.

The dp02 and dp03 data are used in storage calculations, and the dp04 data 
include both the storage and turbulent components. Since many users will 
want to focus on the net flux data, we'll start there.

### Extract Level 4 data (Fluxes!)

To extract the Level 4 data from the HDF5 files and merge them into a 
single table, we'll use the `stackEddy()` function from the `neonUtilities` 
package.

`stackEddy()` requires two inputs:

* `filepath`: Path to a file or folder, which can be any one of:
    1. A zip file of eddy flux data downloaded from the NEON data portal
    2. A folder of eddy flux data downloaded by the `zipsByProduct()` function
    3. The folder of files resulting from unzipping either of 1 or 2
    4. A single HDF5 file of NEON eddy flux data
* `level`: dp01-4

Input the filepath you downloaded to using `zipsByProduct()` earlier, 
including the `filestoStack00200` folder created by the function, and 
`dp04`:



```r
flux <- stackEddy(filepath="./data/filesToStack00200",
                 level="dp04")
```



We now have an object called `flux`. It's a named list containing four 
tables: one table for each site's data, and `variables` and `objDesc` 
tables.



```r
names(flux)
```


Let's look at the contents of one of the site data files:



```r
knitr::kable(head(flux$NIWO))
```


The `variables` and `objDesc` tables can help you interpret the column 
headers in the data table. The `objDesc` table contains definitions for 
many of the terms used in the eddy flux data product, but it isn't 
complete. To get the terms of interest, we'll break up the column headers 
into individual terms and look for them in the `objDesc` table:



```r
term <- unlist(strsplit(names(flux$NIWO), split=".", fixed=T))
flux$objDesc[which(flux$objDesc$Object %in% term),]
knitr::kable(term)
```


For the terms that aren't captured here, `fluxCo2`, `fluxH2o`, and `fluxTemp` 
are self-explanatory. The flux components are

* `turb`: Turbulent flux
* `stor`: Storage
* `nsae`: Net surface-atmosphere exchange

The `variables` table contains the units for each field:



```r
knitr::kable(flux$variables)
```




Let's plot some data! First, we'll need to convert the time stamps 
to an R date-time format (right now they're just character fields).

### Time stamps

NEON sensor data come with time stamps for both the start and end of 
the averaging period. Depending on the analysis you're doing, you may 
want to use one or the other; for general plotting, re-formatting, and 
transformations, I prefer to use the start time, because there 
are some small inconsistencies between data products in a few of the 
end time stamps.

Note that **all** NEON data use UTC time, noted as 
`tz="GMT"` in the code below. This is true across NEON's instrumented, 
observational, and airborne measurements. When working with NEON data, 
it's best to keep everything in UTC as much as possible, otherwise it's 
very easy to end up with data in mismatched times, which can cause 
insidious and hard-to-detect problems. Be sure to include the `tz` 
argument in all the lines of code below - if there is no time zone 
specified, R will default to the local time zone it detects on your 
operating system.



```r
timeB <- as.POSIXct(flux$NIWO$timeBgn, 
                    format="%Y-%m-%dT%H:%M:%S", 
                    tz="GMT")
flux$NIWO <- cbind(timeB, flux$NIWO)
```



```r
plot(flux$NIWO$data.fluxCo2.nsae.flux~timeB, 
     pch=".", xlab="Date", ylab="CO2 flux",
     xaxt="n")
axis.POSIXct(1, x=timeB, format="%Y-%m-%d")
```


Like a lot of flux data, these data have some stray spikes, but there 
is a clear diurnal pattern going into the growing season.

Let's trim down to just two days of data to see a few other details.



```r
plot(flux$NIWO$data.fluxCo2.nsae.flux~timeB, 
     pch=20, xlab="Date", ylab="CO2 flux",
     xlim=c(as.POSIXct("2018-07-07", tz="GMT"),
            as.POSIXct("2018-07-09", tz="GMT")),
    ylim=c(-20,20), xaxt="n")
axis.POSIXct(1, x=timeB, format="%Y-%m-%d %H:%M:%S")
```



Note the timing of C uptake; the UTC time zone is clear here, where 
uptake occurs at times that appear to be during the night.

### Merge flux data with other sensor data

Many of the data sets we would use to interpret and model flux data are 
measured as part of the NEON project, but are not present in the eddy flux 
data product bundle. In this section, we'll download PAR data and merge 
them with the flux data; the steps taken here can be applied to any of the 
NEON instrumented (IS) data products.

#### Download PAR data

To get NEON PAR data, use the `loadByProduct()` function from the 
`neonUtilities` package. `loadByProduct()` takes the same inputs as 
`zipsByProduct()`, but it loads the downloaded data directly into the 
current R environment.

Let's download PAR data matching the Niwot Ridge flux data. The inputs 
needed are:

* `dpID`: DP1.00024.001
* `site`: NIWO
* `startdate`: 2018-06
* `enddate`: 2018-07
* `package`: basic
* `avg`: 30

The new input here is `avg=30`, which downloads only the 30-minute data. 
Since the flux data are at a 30-minute resolution, we can save on 
download time by disregarding the 1-minute data files (which are of course 
30 times larger). The `avg` input can be left off if you want to download 
all available averaging intervals.



```r
pr <- loadByProduct("DP1.00024.001", site="NIWO", avg=30,
                    startdate="2018-06", enddate="2018-07",
                    package="basic", check.size=F)
```



`pr` is another named list, and again, metadata and units can be found in 
the `variables` table. The `PARPAR_30min` table contains a `verticalPosition` 
field. This field indicates the position on the tower, with 10 being the 
first tower level, and 20, 30, etc going up the tower.

#### Join PAR to flux data

We'll connect PAR data from the tower top to the flux data.



```r
pr.top <- pr$PARPAR_30min[which(pr$PARPAR_30min$verticalPosition==
                                max(pr$PARPAR_30min$verticalPosition)),]
```

`loadByProduct()` automatically converts time stamps when it reads the 
data, so here we just need to indicate which time field to use to 
merge the flux and PAR data.



```r
timeB <- pr.top$startDateTime
pr.top <- cbind(timeB, pr.top)
```

And merge the two datasets:



```r
fx.pr <- merge(pr.top, flux$NIWO, by="timeB")
```



```r
plot(fx.pr$data.fluxCo2.nsae.flux~fx.pr$PARMean,
     pch=".", ylim=c(-20,20),
     xlab="PAR", ylab="CO2 flux")
```




If you're interested in data in the eddy covariance bundle besides the 
net flux data, the rest of this tutorial will guide you through how to 
get those data out of the bundle.

### Vertical profile data (Level 3)

The Level 3 (`dp03`) data are the spatially interpolated profiles of 
the rates of change of CO<sub>2</sub>, H<sub>2</sub>O, and temperature.
Extract the Level 3 data from the HDF5 file using `stackEddy()` with 
the same syntax as for the Level 4 data.



```r
prof <- stackEddy(filepath="./data/filesToStack00200/",
                 level="dp03")
```



```r
knitr::kable(head(prof$NIWO))
```


### Un-interpolated vertical profile data (Level 2)

The Level 2 data are interpolated in time but not in space. They 
contain the rates of change at the measurement heights.

Again, they can be extracted from the HDF5 files using `stackEddy()` 
with the same syntax:



```r
prof.l2 <- stackEddy(filepath="./data/filesToStack00200/",
                 level="dp02")
```





```r
knitr::kable(head(prof.l2$HARV))
```



Note that here, as in the PAR data, there is a `verticalPosition` field. 
It has the same meaning as in the PAR data, indicating the tower level of 
the measurement.

### Calibrated raw data (Level 1)

Level 1 (`dp01`) data are calibrated, and aggregated in time, but 
otherwise untransformed. Use Level 1 data for raw gas 
concentrations and atmospheric stable isotopes.

Using `stackEddy()` to extract Level 1 data requires additional 
inputs. The Level 1 files are too large to simply pull out all the 
variables by default, and they include mutiple averaging intervals, 
which can't be merged. So two additional inputs are needed:

* `avg`: The averaging interval to extract
* `var`: One or more variables to extract

What variables are available, at what averaging intervals? Another 
function in the `neonUtilities` package, `getVarsEddy()`, returns 
a list of HDF5 file contents. It requires only one input, a filepath 
to a single NEON HDF5 file:



```r
vars <- getVarsEddy("./data/filesToStack00200/NEON.D01.HARV.DP4.00200.001.nsae.2018-07.basic.h5")
knitr::kable(head(vars))
```




Inputs to `var` can be any values from the `name` field in the table 
returned by `getVarsEddy()`. Let's take a look at CO<sub>2</sub> and 
H<sub>2</sub>O, <sup>13</sup>C in CO<sub>2</sub> and <sup>18</sup>O in 
H<sub>2</sub>O, at 30-minute aggregation. Let's look at Harvard Forest 
for these data, since deeper canopies generally have more interesting 
profiles:



```r
iso <- stackEddy(filepath="./data/filesToStack00200/",
               level="dp01", var=c("rtioMoleDryCo2","rtioMoleDryH2o",
                                   "dlta13CCo2","dlta18OH2o"), avg=30)
```





```r
knitr::kable(head(iso$HARV))
```




Let's plot vertical profiles of CO<sub>2</sub> and <sup>13</sup>C in CO<sub>2</sub> 
on a single day. 

Here, for convenience, instead of converting the time stamps 
to a time format, it's easy to use the character format to extract the ones 
we want using `grep()`. And discard the `verticalPosition` values that are 
string values - those are the calibration gases.



```r
iso.d <- iso$HARV[grep("2018-06-25", iso$HARV$timeBgn, fixed=T),]
iso.d <- iso.d[-which(is.na(as.numeric(iso.d$verticalPosition))),]
```




`ggplot` is well suited to these types of data, let's use it to plot 
the profiles.



```r
library(ggplot2)
```



```r
g <- ggplot(iso.d, aes(y=verticalPosition)) + 
  geom_path(aes(x=data.co2Stor.rtioMoleDryCo2.mean, 
                group=timeBgn, col=timeBgn)) + 
  theme(legend.position="none") + 
  xlab("CO2") + ylab("Tower level")
g
```




<img src="./images/eddy_intro_50_1.png" width="420" />




```r
g <- ggplot(iso.d, aes(y=verticalPosition)) + 
  geom_path(aes(x=data.isoCo2.dlta13CCo2.mean, 
                group=timeBgn, col=timeBgn)) + 
  theme(legend.position="none") + 
  xlab("d13C") + ylab("Tower level")
g
```

    Warning message:
    “Removed 55 rows containing missing values (geom_path).”
    

<img src="./images/eddy_intro_51_1.png" width="420" />


The legends are omitted for space, see if you can work out the times 
of day the different colors represent.


### Convert NEON flux data variables to AmeriFlux FP standard

Install and load packages


```r
#Install NEONprocIS.base from GitHub, this package is a dependency of eddy4R.base

devtools::install_github(repo="NEONScience/NEON-IS-data-processing",
                         ref="master",
                         subdir="pack/NEONprocIS.base",
                         dependencies=c(NA, TRUE)[2],
                         repos=c(BiocManager::repositories(),   # for dependencies on Bioconductor packages
                                 "https://cran.rstudio.com/")       # for CRAN
)



#Install eddy4R.base from GitHub

devtools::install_github(repo="NEONScience/eddy4R",
                         ref="master",
                         subdir="pack/eddy4R.base",
                         dependencies=c(NA, TRUE)[2],
                         repos=c(BiocManager::repositories(),   # for dependencies on Bioconductor packages
                                 "https://cran.rstudio.com/")       # for CRAN
)

packReq <- c("rhdf5", "eddy4R.base", "jsonlite", "lubridate")

lapply(packReq, function(x) {
  print(x)
  if(require(x, character.only = TRUE) == FALSE) {
    install.packages(x)
    library(x, character.only = TRUE)
  }})
```


Select your site of interest from the list of NEON sites below.  


```r
site <- "KONZ"
  
  #"BARR","CLBJ","MLBS","DSNY","NIWO","ORNL","OSBS",
  #"SCBI","LENO","TALL","CPER","BART","HARV","BLAN",
  #"SERC","JERC","GUAN","LAJA","STEI","TREE","UNDE",
  #"KONA","KONZ","UKFS","GRSM","DELA","DCFS","NOGP",
  #"WOOD","RMNP","OAES","YELL","MOAB","STER","JORN",
  #"SRER","ONAQ","ABBY","WREF","SJER","SOAP","TEAK",
  #"TOOL","BONA","DEJU","HEAL","PUUM"
}
```

If you would like to download a set range of dates, define the following paramemters. If these are not defined, it will default to the entire record at the site


```r
#define start and end dates, optional, defaults to entire period of site operation. Use %Y-%m-%d format.
dateBgn <- "2020-03-01"
dateEnd <- "2020-05-31"

# Data package from the portal
Pack <- c('basic','expanded')[1]
#The version data for the FP standard conversion processing
ver = paste0("v",format(Sys.time(), "%Y%m%dT%H%m"))
```


Specify Download directory for HDF5 files from the NEON data portal and output directory to save the resulting csv files. Change save paths to where you want the files on your computer. 


```r
#download directory
DirDnld=tempdir()

#Output directory, change this to where you want to save the output csv
DirOutBase <-paste0("~/eddy/data/Ameriflux/",ver)
```

Specify Data Product number, for the Bundled Eddy-Covariance files, this is DP4.00200.001 


```r
#DP number
dpID <- 'DP4.00200.001'
```


Get metadata from Ameriflux Site Info BADM sheets for the site of interest
  

```r
  #Grab a list of all Ameriflux sites, containing site ID and site description
  sites_web <- jsonlite::fromJSON("http://ameriflux-data.lbl.gov/AmeriFlux/SiteSearch.svc/SiteList/AmeriFlux")
  
  #Grab only NEON sites
  sitesNeon <- sites_web[grep(pattern = paste0("NEON.*",site), x = sites_web$SITE_NAME),] #For all NEON sites
  siteNeon <- sites_web[grep(pattern = paste0("NEON.*",site), x = sites_web$SITE_NAME),]
  
  metaSite <- lapply(siteNeon$SITE_ID, function(x) {
    pathSite <- paste0("http://ameriflux-data.lbl.gov/BADM/Anc/SiteInfo/",x)
    tmp <- fromJSON(pathSite)
    return(tmp)
    }) 
```
  
  
Use Ameriflux site IDs to name metadata lists

```r
#use NEON ID as list name
  names(metaSite) <- site 
#Use Ameriflux site ID as list name  
  #names(metaSite) <- sitesNeon$SITE_ID 
```

Check if dateBgn is defined, if not make it the initial operations date "IOCR" of the site


```r
  if(!exists("dateBgn") || is.na(dateBgn) || is.null(dateBgn)){
    dateBgn <- as.Date(metaSite[[site]]$values$GRP_FLUX_MEASUREMENTS[[1]]$FLUX_MEASUREMENTS_DATE_START, "%Y%m%d")
  } else {
    dateBgn <- dateBgn
  }#End of checks for missing dateBgn
  
  #Check if dateEnd is defined, if not make it the system date
  if(!exists("dateEnd") || is.na(dateEnd) || is.null(dateEnd)){
    dateEnd <- as.Date(Sys.Date())
  } else {
    dateEnd <- dateEnd
  }#End of checks for missing dateEnd
```

Grab the UTC time offset from the Ameriflux API

```r
  timeOfstUtc <- as.integer(metaSite[[site]]$values$GRP_UTC_OFFSET[[1]]$UTC_OFFSET)
```

Create the date sequence

```r
  setDate <- seq(from = as.Date(dateBgn), to = as.Date(dateEnd), by = "month")
```
  

Start processing the site time range specified, verify that the site and date range are specified as intended

```r
  msg <- paste0("Starting Ameriflux FP standard conversion processing workflow for ", site, " for ", dateBgn, " to ", dateEnd)
  print(msg)
```

Create output directory by checking if the download directory exists and create it if not

```r
  if(dir.exists(DirDnld) == FALSE) dir.create(DirDnld, recursive = TRUE)
  #Append the site to the base output directory
  DirOut <- paste0(DirOutBase, "/", siteNeon$SITE_ID)
  #Check if directory exists and create if not
  if(!dir.exists(DirOut)) dir.create(DirOut, recursive = TRUE)
```

Download and extract data

```r
  #Initialize data List
  dataList <- list()
  
  #Read data from the API
  dataList <- lapply(setDate, function(x) {
    # year <- lubridate::year(x)
    # mnth <- lubridate::month(x)
    date <- stringr::str_extract(x, pattern = paste0("[0-9]{4}", "-", "[0-9]{2}"))
    tryCatch(neonUtilities::zipsByProduct(dpID = dpID, site = site, startdate = date, enddate = date, package = "basic", savepath = DirDnld, check.size = FALSE), error=function(e) NULL)
    files <- list.files(paste0(DirDnld, "/filesToStack00200"))
    utils::unzip(paste0(DirDnld, "/filesToStack00200/", files[grep(pattern = paste0(site,".*.", date, ".*.zip"), x = files)]), exdir = paste0(DirDnld, "/filesToStack00200"))
    files <- list.files(paste0(DirDnld, "/filesToStack00200"))
    dataIdx <- rhdf5::h5read(file = paste0(DirDnld, "/filesToStack00200/", max(files[grep(pattern = paste0(site,".*.", date,".*.h5"), x = files)])), name = paste0(site, "/"))
                      
    if(!is.null(dataIdx)){ 
       dataIdx$dp0p <- NULL 
       dataIdx$dp02 <- NULL 
       dataIdx$dp03 <- NULL
       dataIdx$dp01$ucrt <- NULL 
       dataIdx$dp04$ucrt <- NULL 
       dataIdx$dp01$data <- lapply(dataIdx$dp01$data,FUN=function(var){ 
         nameTmi <- names(var) 
         var <- var[grepl('_30m',nameTmi)] 
         return(var)})
       dataIdx$dp01$qfqm <- lapply(dataIdx$dp01$qfqm,FUN=function(var){ 
         nameTmi <- names(var)
         var <- var[grepl('_30m',nameTmi)]
         return(var)})
    }
    return(dataIdx)
  })
```

  
Add names to list for year/month combinations
  

```r
names(dataList) <- paste0(lubridate::year(setDate),sprintf("%02d",lubridate::month(setDate)))
```
  
  
Remove NULL elements from list

```r
dataList <- dataList[vapply(dataList, Negate(is.null), NA)]
```

Determine tower horizontal & vertical indices

```r
    #Find the tower top level by looking at the vertical index of the turbulent CO2 concentration measurements 
    LvlTowr <- grep(pattern = "_30m", names(dataList[[1]]$dp01$data$co2Turb), value = TRUE)
    LvlTowr <- gsub(x = LvlTowr, pattern = "_30m", replacement = "")
    
    #get tower top level
    LvlTop <- strsplit(LvlTowr,"")
    LvlTop <- base::as.numeric(LvlTop[[1]][6])
    
    #Ameriflux vertical levels based off of https://ameriflux.lbl.gov/data/aboutdata/data-variables/ section 3.3.1 "Indices must be in order, starting with the highest."
    idxVerAmfx <- base::seq(from = 1, to = LvlTop, by = 1)
    #get the sequence from top to first level
    LvlMeas <- base::seq(from = LvlTop, to = 1, by = -1)
    #Recreate NEON naming conventions
    LvlMeas <- paste0("000_0",LvlMeas,"0",sep="")
    #Give NEON naming conventions to Ameriflux vertical levels
    names(idxVerAmfx) <- LvlMeas
    
    #Ameriflux horizontal index
    idxHorAmfx <- 1
```
    
Subset to the Ameriflux variables to convert

```r
    dataListFlux <- lapply(names(dataList), function(x) {
      data.frame(
        "TIMESTAMP_START" = as.POSIXlt(dataList[[x]]$dp04$data$fluxCo2$turb$timeBgn, format="%Y-%m-%dT%H:%M:%OSZ", tz = "GMT"),
        "TIMESTAMP_END" = as.POSIXlt(dataList[[x]]$dp04$data$fluxCo2$turb$timeEnd, format="%Y-%m-%dT%H:%M:%OSZ", tz = "GMT"),
        # "TIMESTAMP_START" = strftime(as.POSIXlt(dataList[[x]][[idxSite]]$dp04$data$fluxCo2$turb$timeBgn, format="%Y-%m-%dT%H:%M:%OSZ"), format = "%Y%m%d%H%M"),
        # "TIMESTAMP_END" = strftime(as.POSIXlt(dataList[[x]][[idxSite]]$dp04$data$fluxCo2$turb$timeEnd, format="%Y-%m-%dT%H:%M:%OSZ") + 60, format = "%Y%m%d%H%M"),
        "FC"= dataList[[x]]$dp04$data$fluxCo2$turb$flux,
        "SC"= dataList[[x]]$dp04$data$fluxCo2$stor$flux,
        "NEE"= dataList[[x]]$dp04$data$fluxCo2$nsae$flux,
        "LE" = dataList[[x]]$dp04$data$fluxH2o$turb$flux,
        "SLE" = dataList[[x]]$dp04$data$fluxH2o$stor$flux,
        "USTAR" = dataList[[x]]$dp04$data$fluxMome$turb$veloFric,
        
        "H" = dataList[[x]]$dp04$data$fluxTemp$turb$flux,
        "SH" = dataList[[x]]$dp04$data$fluxTemp$stor$flux,
        "FETCH_90" = dataList[[x]]$dp04$data$foot$stat$distXaxs90,
        "FETCH_MAX" = dataList[[x]]$dp04$data$foot$stat$distXaxsMax,
        "V_SIGMA" = dataList[[x]]$dp04$data$foot$stat$veloYaxsHorSd,
        #"W_SIGMA" = dataList[[x]]$dp04$data$foot$stat$veloZaxsHorSd,
        "CO2_1_1_1" = dataList[[x]]$dp01$data$co2Turb[[paste0(LvlTowr,"_30m")]]$rtioMoleDryCo2$mean,
        "H2O_1_1_1" = dataList[[x]]$dp01$data$h2oTurb[[paste0(LvlTowr,"_30m")]]$rtioMoleDryH2o$mean,
        "qfFinlH2oTurbFrt00Samp" = dataList[[x]]$dp01$qfqm$h2oTurb[[paste0(LvlTowr,"_30m")]]$frt00Samp$qfFinl,
        "qfH2O_1_1_1" = dataList[[x]]$dp01$qfqm$h2oTurb[[paste0(LvlTowr,"_30m")]]$rtioMoleDryH2o$qfFinl,
        "qfCO2_1_1_1" = dataList[[x]]$dp01$qfqm$co2Turb[[paste0(LvlTowr,"_30m")]]$rtioMoleDryCo2$qfFinl,
        "qfSC" = dataList[[x]]$dp04$qfqm$fluxCo2$stor$qfFinl,
        "qfSLE" = dataList[[x]]$dp04$qfqm$fluxH2o$stor$qfFinl,
        "qfSH" = dataList[[x]]$dp04$qfqm$fluxTemp$stor$qfFinl,
        "qfT_SONIC" = dataList[[x]]$dp01$qfqm$soni[[paste0(LvlTowr,"_30m")]]$tempSoni$qfFinl,
        "qfWS_1_1_1" = dataList[[x]]$dp01$qfqm$soni[[paste0(LvlTowr,"_30m")]]$veloXaxsYaxsErth$qfFinl,
        rbind.data.frame(lapply(names(idxVerAmfx), function(y) {
          tryCatch({rlog$debug(y)}, error=function(cond){print(y)})
          rpt <- list()
          rpt[[paste0("CO2_1_",idxVerAmfx[y],"_2")]] <- dataList[[x]]$dp01$data$co2Stor[[paste0(y,"_30m")]]$rtioMoleDryCo2$mean
          
          
          rpt[[paste0("H2O_1_",idxVerAmfx[y],"_2")]] <- dataList[[x]]$dp01$data$h2oStor[[paste0(y,"_30m")]]$rtioMoleDryH2o$mean
          rpt[[paste0("CO2_1_",idxVerAmfx[y],"_3")]] <- dataList[[x]]$dp01$data$isoCo2[[paste0(y,"_30m")]]$rtioMoleDryCo2$mean
          
          rpt[[paste0("H2O_1_",idxVerAmfx[y],"_3")]] <- dataList[[x]]$dp01$data$isoCo2[[paste0(y,"_30m")]]$rtioMoleDryH2o$mean
          rpt[[paste0("qfCO2_1_",idxVerAmfx[y],"_2")]] <- dataList[[x]]$dp01$qfqm$co2Stor[[paste0(LvlTowr,"_30m")]]$rtioMoleDryCo2$qfFinl
          rpt[[paste0("qfH2O_1_",idxVerAmfx[y],"_2")]] <- dataList[[x]]$dp01$qfqm$h2oStor[[paste0(LvlTowr,"_30m")]]$rtioMoleDryH2o$qfFinl
          rpt[[paste0("qfCO2_1_",idxVerAmfx[y],"_3")]] <- dataList[[x]]$dp01$qfqm$isoCo2[[paste0(LvlTowr,"_30m")]]$rtioMoleDryCo2$qfFinl
          rpt[[paste0("qfH2O_1_",idxVerAmfx[y],"_3")]] <- dataList[[x]]$dp01$qfqm$isoH2o[[paste0(LvlTowr,"_30m")]]$rtioMoleDryH2o$qfFinl
          
          rpt <- rbind.data.frame(rpt)
          return(rpt)
        }
        )),
        
        
        "WS_1_1_1" = dataList[[x]]$dp01$data$soni[[paste0(LvlTowr,"_30m")]]$veloXaxsYaxsErth$mean,
        "WS_MAX_1_1_1" = dataList[[x]]$dp01$data$soni[[paste0(LvlTowr,"_30m")]]$veloXaxsYaxsErth$max,
        "WD_1_1_1" = dataList[[x]]$dp01$data$soni[[paste0(LvlTowr,"_30m")]]$angZaxsErth$mean,
        "T_SONIC" = dataList[[x]]$dp01$data$soni[[paste0(LvlTowr,"_30m")]]$tempSoni$mean,
        "T_SONIC_SIGMA" = base::sqrt(dataList[[x]]$dp01$data$soni[[paste0(LvlTowr,"_30m")]]$tempSoni$mean)
        , stringsAsFactors = FALSE)
    })
    
    names(dataListFlux) <- names(dataList)
```

Combine the monthly data into a single dataframe, remove lists and clean memory

```r
    dataDfFlux <- do.call(rbind.data.frame,dataListFlux)
    rm(list=c("dataListFlux","dataList"))
    gc()
```

Regularize timeseries to 30 minutes in case timestamps are missing from NEON files due to processing errors

```r
    timeRglr <- eddy4R.base::def.rglr(timeMeas = as.POSIXlt(dataDfFlux$TIMESTAMP_START), dataMeas = dataDfFlux, BgnRglr = as.POSIXlt(dataDfFlux$TIMESTAMP_START[1]), EndRglr = as.POSIXlt(dataDfFlux$TIMESTAMP_END[length(dataDfFlux$TIMESTAMP_END)]), TzRglr = "UTC", FreqRglr = 1/(60*30))
    
    #Reassign data to data.frame
    dataDfFlux <- timeRglr$dataRglr
    #Format timestamps
    dataDfFlux$TIMESTAMP_START <- strftime(timeRglr$timeRglr + lubridate::hours(timeOfstUtc), format = "%Y%m%d%H%M")
    dataDfFlux$TIMESTAMP_END <- strftime(timeRglr$timeRglr + lubridate::hours(timeOfstUtc) + lubridate::minutes(30), format = "%Y%m%d%H%M")
```

Define validation times, and remove this data from the dataset. At NEON sites, validations with a series of gasses of known concentration are run every 23.5 hours. These values are used to correct for measurment drift and are run every 23.5 hours to achive daily resolution while also spreading the impact of lost measurements throughout the day. 


```r
    #Remove co2Turb and h2oTurb data based off of qfFlow (qfFinl frt00)
    dataDfFlux$FC[(which(dataDfFlux$qfCO2_1_1_1 == 1))] <- NaN
    dataDfFlux$LE[(which(dataDfFlux$qfH2O_1_1_1 == 1))] <- NaN
    dataDfFlux$USTAR[(which(dataDfFlux$qfWS_1_1_1 == 1))] <- NaN
    dataDfFlux$H[(which(dataDfFlux$qfT_SONIC_1_1_1 == 1))] <- NaN
    dataDfFlux$SC[(which(dataDfFlux$qfSC == 1))] <- NaN
    dataDfFlux$SLE[(which(dataDfFlux$qfSLE == 1))] <- NaN
    dataDfFlux$SH[(which(dataDfFlux$qfSH == 1))] <- NaN
    dataDfFlux$T_SONIC[(which(dataDfFlux$qfT_SONIC_1_1_1 == 1))] <- NaN
    dataDfFlux$T_SONIC_SIGMA[(which(dataDfFlux$qfT_SONIC_1_1_1 == 1))] <- NaN
    dataDfFlux$WS_1_1_1[(which(dataDfFlux$qfWS_1_1_1 == 1))] <- NaN
    dataDfFlux$WS_MAX_1_1_1[(which(dataDfFlux$qfWS_1_1_1 == 1))] <- NaN
    dataDfFlux$WD_1_1_1[(which(dataDfFlux$qfWS_1_1_1 == 1))] <- NaN
    
    dataDfFlux$H2O_1_1_1[(which(dataDfFlux$qfH2O_1_1_1 == 1))] <- NaN
    dataDfFlux$CO2_1_1_1[(which(dataDfFlux$qfCO2_1_1_1 == 1))] <- NaN
    
    lapply(idxVerAmfx, function(x){
      #x <- 1
      dataDfFlux[[paste0("H2O_1_",x,"_2")]][(which(dataDfFlux[[paste0("qfH2O_1_",x,"_2")]] == 1))] <<- NaN
      dataDfFlux[[paste0("H2O_1_",x,"_3")]][(which(dataDfFlux[[paste0("qfH2O_1_",x,"_3")]] == 1))] <<- NaN
      dataDfFlux[[paste0("CO2_1_",x,"_2")]][(which(dataDfFlux[[paste0("qfCO2_1_",x,"_2")]] == 1))] <<- NaN
      dataDfFlux[[paste0("CO2_1_",x,"_3")]][(which(dataDfFlux[[paste0("qfCO2_1_",x,"_3")]] == 1))] <<- NaN
    })
```

Remove quality flagging variables from output

```r
    setIdxQf <- grep("qf", names(dataDfFlux))
    dataDfFlux[,setIdxQf] <- NULL
```

Set range thresholds

```r
    #assign list
    Rng <- list()
    
    Rng$Min <- data.frame(
      "FC" = -100,            #[umol m-2 s-1]
      "SC" = -100,            #[umol m-2 s-1]
      "NEE" = -100,            #[umol m-2 s-1]
      "LE" = -500,            #[W m-2]
      "H" = -500,             #[W m-2]
      "USTAR" = 0,            #[m s-1]
      "CO2" = 200,            #[umol mol-1]
      "H2O" = 0,              #[mmol mol-1]
      "WS_1_1_1" = 0,         #[m s-1]
      "WS_MAX_1_1_1" = 0,     #[m s-1]
      "WD_1_1_1" = -0.1,      #[deg]
      "T_SONIC" = -55.0       #[C]
    )
```

    
Set Max thresholds

```r
    Rng$Max <- data.frame(
      "FC" = 100,            #[umol m-2 s-1]
      "SC" = 100,            #[umol m-2 s-1]
      "NEE" = 100,            #[umol m-2 s-1]
      "LE" = 1000,            #[W m-2]
      "H" = 1000,             #[W m-2]
      "USTAR" = 5,            #[m s-1]
      "CO2" = 800,            #[umol mol-1]
      "H2O" = 100,              #[mmol mol-1]
      "WS_1_1_1" = 50,         #[m s-1]
      "WS_MAX_1_1_1" = 50,     #[m s-1]
      "WD_1_1_1" = 360,      #[deg]
      "T_SONIC" = 45.0       #[C]
    )
```

Grab all CO2/H2O columns to apply same thresholds, replace missing values with -9999

```r
    nameCO2 <- grep("CO2",names(dataDfFlux),value = TRUE)
    nameH2O <- grep("H2O",names(dataDfFlux),value = TRUE)
    #Apply the CO2/H2O threshold to all variables in HOR_VER_REP
    Rng$Min[nameCO2] <- Rng$Min$CO2
    Rng$Min[nameH2O] <- Rng$Min$H2O
    Rng$Max[nameCO2] <- Rng$Max$CO2
    Rng$Max[nameH2O] <- Rng$Max$H2O
    
    #Apply the range test to the output, and replace values with NaN
    lapply(names(dataDfFlux), function(x) {
      dataDfFlux[which(dataDfFlux[,x]<Rng$Min[[x]] | dataDfFlux[,x]>Rng$Max[[x]]),x] <<- NaN})
    
    # Delete any NEE that have either FC or SC removed
    dataDfFlux[is.na(dataDfFlux$FC) | is.na(dataDfFlux$SC),"NEE"] <- NaN
    
    #Change NA to -9999
    dataDfFlux[is.na(dataDfFlux)] <- -9999
```

Write output data to csv

```r
    #Create output filename based off of Ameriflux file naming convention
    nameFileOut <- base::paste0(DirOut,"/",siteNeon$SITE_ID,'_HH_',dataDfFlux$TIMESTAMP_START[1],'_',utils::tail(dataDfFlux$TIMESTAMP_END,n=1),'_flux.csv')
    
    #Write output to .csv
    write.csv(x = dataDfFlux, file = nameFileOut, row.names = FALSE)
```

Clean up environment

```r
  rm(list="dataDfFlux")
  gc()
```


## Exercises

### Computational


1) NEON data are submitted to AmeriFlux quarterly after one year of non-quality flagged or otherwise missing data are available. Use the workflow above to extend the data coverage of an already submitted NEON site by downloading existing data from the AmeriFlux website and recently published HDF5 files from the NEON data portal.  Process the NEON data such that it is in AmeriFlux format and plot the entire timerseries.

*Hint: NEON sites start with US-x*


2) Using metScanR package, find co-located NEON and AmeriFlux sites. Download data for an overlapping time period, and compare FC and H values by making a scatter plot and seeing how far off the data are from a 1:1 line. 




<!--chapter:end:06-Fluxes_and_Inter-operability.Rmd-->


# NEON AOP

Placeholder


## Hyperspectral Remote Sensing
### Learning Objectives
#### Mapping the Invisible
### About Hyperspectral Remote Sensing Data
## Key Metadata for Hyperspectral Data
### Bands and Wavelengths
### Spectral Resolution
### Full Width Half Max (FWHM)
## Intro to Working with Hyperspectral Remote Sensing Data in HDF5 Format
### Learning Objectives
### R Libraries to Install:
### Data to Download
## About Hyperspectral Remote Sensing Data
##  Read HDF5 data into R
### Bands and Wavelengths
### A Note About Data Slicing in HDF5
### Arrays vs. Matrices
### Dimensions in Arrays
### Data Ignore Value
### Reflectance Values and Image Stretch
### Transpose Image
## Create a Georeferenced Raster
### Define Raster CRS
### Challenge: Work with Rasters
## Light Detection And Ranging (LiDAR) Data
## Calculating Forest Structural Diversity Metrics from NEON LiDAR Data
### Learning Objectives
### R Libraries to Install:
### Data to Download
### Recommended Skills
### Additional Resources
## Introduction to Structural Diversity Metrics
## NEON AOP Discrete Return LIDAR
### Loading the LIDAR Products
### Normalizing Tree Height to Ground
## Calculating Structural Diversity Metrics
### GENERATE CANOPY HEIGHT MODEL (CHM) 
#### MEAN OUTER CANOPY HEIGHT (MOCH)
#### MAX CANOPY HEIGHT
#### RUMPLE
#### TOP RUGOSITY
#### DEEP GAPS & DEEP GAP FRACTION
#### COVER FRACTION
#### HEIGHT SD
#### ENTROPY
#### GAP FRACTION PROFILE 
#### VAI
#### VCI
### Combining Everything Into One Function
### Comparing Metrics Between Forests
## Matching GEDI waveforms with NEON AOP LiDAR pointclouds
### Learning Objectives 
### Things You’ll Need To Complete This GEDI Section
### R Packages to Install
### Example Data Set
#### GEDI Example Data Subset
#### Datum difference between WGS84 and NAD83
#### Datum difference between GEOID12A and NAD83
### Getting Started
### Downloading GEDI data
### Plot GEDI footprints on CHM
### Extract Waveform for a single Shot
### Download and Plot NEON AOP LiDAR pointcloud data
### Clip AOP LiDAR Pointcloud to GEDI footprints
### Plot GEDI Waveform with AOP Pointcloud in 3D space
### Datum, Geoid, and how to best measure the Earth
#### WGS84
#### GEOID12A
### Aligning the Vertical Datum
### GEOID12A Height Model
### Extract vertical offset for GEDI shots
### Plot vertically corrected GEDI waveform in 3D
### Optional - NEON base plots
## NEON AOP Written Questions:
## NEON AOP Coding Lab
## NEON AOP Culmination Write Up

<!--chapter:end:07-NEON_AOP.Rmd-->


# NASA's Earth Observing System (EOS)

Placeholder


## Learning Objectives
## NASA EOS Project Mission & Design
## NASA EOS Earth Data Account:
## **NASA EOS Coding Assignment 1**
## Distributed Active Archive Centers
### LP DAAC
## The LPDAAC Mission: Process, Archive, Distribute, Apply
### How you can use LP DAAC's data
## AppEEARS
## Hands on: Pulling AppEEARS Data via the API
## Getting Started with the AppEEARS API (Point Request)
### Example: Submit a point request for multiple NEON sites to extract vegetation and land surface temperature data   
#### Data Used in the Example:
## Topics Covered in this section:
### Prerequisites:
#### Getting Started:
### AppEEARS Information:
## Getting Started with the AppEEARS API       
### Load Packages
### Set Up the Output Directory
### Login to Earth Data
## Query Available Products
## Search and Explore Available Products
## Search and Explore Available Layers 
## Submit a Point Request
### Compile a JSON Object
### Submit a Task Request
### Retrieve Task Status
## Download a Request
### Explore Files in Request Output 
## Download Files in a Request (Automation) 
## Explore AppEEARS Quality Service
### List Quality Layers 
### Inspect Quality Values 
## Decode Quality Values
## Load Request Output and Visualize
## Load a CSV
## Plot Results (Line/Scatter Plots)
## Submit an Area Request
## Submit an area request using a NEON site boundary as the region of interest for extracting elevation, vegetation and land surface temperature data    
#### Data Used in this Example:
### Topics Covered in this Tutorial
### Prerequisites:
### Procedures:
#### Getting Started:
### AppEEARS Information:
## Getting Started with an Area Request     
### Load Packages for an Area Request
## Set Up the Output Directory
## Load your Earth Data Token
## Query Available Products
## Search and Explore Available Products
## Search and Explore Available Layers
## Submit an Area Request
### Load a Shapefile
## Search and Explore Available Projections
## Compile a JSON Object
## Submit a Task Request 
## Retrieve Task Status
## Download a Request
### Explore Files in Request Output 
## Download Files in a Request (Automation) 
## Explore AppEEARS Quality Service
## List Quality Layers 
## Show Quality Values 
## Decode Quality Values
## BONUS: Load Request Output and Visualize
## Load a GeoTIFF
## Plot a GeoTIFF
## NASA EOS Coding Lab #2
## NASA EOS Written Questions
## NASA EOS Culmination Write Up

<!--chapter:end:08-NASA_EOS.Rmd-->


# USGS National Water Information System (NWIS)

Placeholder


## USGS Mission:
## USGS Water Resources Mission:
## Types of USGS NWIS Data
## USGS R Packages: Collaborative and reproducible data analysis using R
### Suggested prerequisite knowledge
### Course outline
### Software requirements
### Lesson Summary
### Lesson Objectives
### Lesson Resources
### Lesson Slide Deck
## Introduction to USGS R Packages
## Data available
## Common NWIS function arguments
## Discovering NWIS data
### whatNWISdata
## Common WQP function arguments
## Discovering WQP data
### readWQPdata + querySummary
### whatWQPsites
## readNWIS functions
### readNWISdata
### readNWISdv
### readNWISgwl
### readNWISmeas
### readNWISpCode
### readNWISpeak
### readNWISqw
### readNWISrating
### readNWISsite
### readNWISstat
### readNWISuse
### readNWISuv
## Additional Features
### Accessing attributes
### Using lists as input
### Helper functions
## readWQP functions
### readWQPdata
### readWQPqw
## Attributes and metadata
## USGS Coding Lab Exercises
### Just how dry was the 2020 monsoon?
## geoKnife - Introduction
## Lesson Summary
## Lesson Objectives
## Lesson Resources
## Remote processing
## geoknife components: fabric, stencil, knife
## Available webdata
### GDP datasets
### Datasets not in GDP
## Available webgeoms
## Available webprocesses
## Setting up a geojob
## Checking the geojob status
## Getting geojob data
## `wait` and `email`
## Putting it all together, mapping precipitation from Tropical Storm Colin
## USGS NWIS Culmination Write Up

<!--chapter:end:08-USGS.Rmd-->


# Frequently Asked Questions: {-}

Placeholder


## Where can I find due dates for assignments?
## How do I submit assignments?
## Do I still have to submit written exercises as .Rmd and .pdf?
## What's better for code, conciseness or readability?
## How find I find resources to navigate the NEON Data Portal?
## How can I best prepare for class and succeed?

<!--chapter:end:15_FAQ.Rmd-->

