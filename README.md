# A persistently low level of atmospheric oxygen in Earth's middle age

This GitHub repository includes R scripts for importing, analyzing, and visualizing the data using R statistical software (http://www.R-project.org/).

## Contents

- [Overview](#overview)
- [Repo Contents](#repo-contents)
- [System Requirements](#system-requirements)
- [Installation Guide](#installation-guide)
- [Demo](#demo)
- [Results](#results)
- [License](./LICENSE)
- [Citation](#citation)

# Overview
Data and code to reproduce the analyses in the manuscript, 
"A persistently low level of atmospheric oxygen in Earth's middle age". 
Data includes publicly-available weather data in addition to primary temperature logger data from instruments deployed underwater in the Farasan Banks region of the Saudi Arabian Red Sea. 
The code does the following analyses: 
(1) compares in situ temperature logger data to satellite-based sea surface temperature (SST), 
(2) tests which SST product works best to reproduce the spatial and temporal patterns in the temperature loggers, 
(3) compares wind and sea surface height (SSH) patterns to the timing of upwelling events,
(4) assesses the broader climate drivers of upwelling (e.g. monsoon winds). 
All figures included in the manuscript are reproduced here.
The figures 2 and 3 in the paper "A persistently low level of atmospheric oxygen in Earth's middle age" were made using R statistical software (http://www.R-project.org/).

# Repo Contents

- [R](./R): `R` package code.
- [docs](./docs): package documentation, and usage of the `lolR` package on many real and simulated data examples.
- [man](./man): package manual for help in R session.
- [tests](./tests): `R` unit tests written using the `testthat` package.
- [vignettes](./vignettes): `R` vignettes for R session html help pages.

# Setting up the development environment:

# System Requirements

## Hardware Requirements

The scripts requires only a standard computer with enough RAM to support the operations defined by a user. For minimal performance, this will be a computer with about 2 GB of RAM. For optimal performance, we recommend a computer with the following specs:

RAM: 16+ GB  
CPU: 4+ cores, 3.3+ GHz/core

The runtimes below are generated using a computer with the recommended specs (16 GB RAM, 4 cores@3.3 GHz) and internet of speed 25 Mbps.

## Software Requirements

### OS Requirements

The developmental version of the scripts has been tested on the following systems:
Windows 10

The CRAN package should be compatible with Windows, Mac, and Linux operating systems.

Before setting up program testing environment, users should have `R` version 3.4.0 or higher, and several packages set up from CRAN.
# Installation Guide
#### Installing R version 3.4.2 on Windows 10

the latest version of R can be installed by following the guilds below:

1. Download R from http://cran.us.r-project.org/.
2. Click on Download R for Windows. Click on base. Click on Download R 3.3.2 for Windows (or a newer version that appears).
3. Install R. Leave all default settings in the installation options.

4. Install RStudio requires R 3.0.1+.

5. Download RStudio Desktop for windows from http://rstudio.org/download/desktop (it should be called something like RStudio Desktop 1.3.1093 — Windows Vista/7/8/10). Choose default installation options.
6. Open RStudio. 
(If you want to learn how to install packages, you can see find some tutorials from the following site or from some books:
https://towardsdatascience.com/setup-a-data-science-environment-on-your-personal-computer-6ce931113914).

total setup time depending on your personal computer system and familar with the R software,
but usually should install within about 10 minues.


## Development Version

### Package dependencies

Users should install the following packages prior to installing `lolR`, from an `R` terminal:

```
install.packages(c('ggplot2', 'abind', 'irlba', 'knitr', 'rmarkdown', 'latex2exp', 'MASS', 'randomForest'))
```

which will install in about 30 seconds on a machine with the recommended specs.

The `lolR` package functions with all packages in their latest versions as they appear on `CRAN` on December 13, 2017. Users can check [CRAN snapshot](https://mran.microsoft.com/timemachine/) for details. The versions of software are, specifically:
```
abind_1.4-5
latex2exp_0.4.0
ggplot2_2.2.1
irlba_2.3.1
Matrix_1.2-3
MASS_7.3-47
randomForest_4.6-12
```

If you are having an issue that you believe to be tied to software versioning issues, please drop us an [Issue](https://github.com/neurodata/lol/issues). 

### Package Installation

From an `R` session, type:

```
require(devtools)
install_github('neurodata/lol', build_vignettes=TRUE, force=TRUE)  # install lol with the vignettes
require(lolR)
vignette("lol", package="lolR")  # view one of the basic vignettes
```

The package should take approximately 40 seconds to install with vignettes on a recommended computer. 

# Demo
## Instructions to run on data
### Figure 2
The R script file named "R_ScriptForFigure2.txt" is used to reproduce the Figure 2 in this paper.
The script has add very detialed comments for almost each line of the code and please check out the code into the R script.

### Figure 3
The R script file named "R_ScriptForFigure3.txt" is used to reproduce the Figure 3 in this paper.




# Results



# Citation

For usage of the scripts and associated manuscript, please cite according to citation of the published paper.
