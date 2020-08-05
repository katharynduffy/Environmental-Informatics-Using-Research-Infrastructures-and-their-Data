# Ecoinformatics Tools

As an Ecoinformatician you *need* to be able to:

1. Pull data from Application Programing Interfaces (APIs)
    + More on this in Chapter 2
2. Organize and document your code and data

3. Version control your code to avoid disaster and make it reproducible
    + For you, your collaborators, and/or the wider community
4. Push your code up to public-facing repositories

5. Pull other's code from public repositories.

More thoughts on the benefits and power of reproducibility [can be found here](https://github.com/katharynduffy/ECOSS_reproducible_science)

To be successful, both in this course and in your careers you will need these skills.  This is why **they are a requirement** for this course.  If you are already using these skills on a daily basis, fantastic!  If you don't feel that you have mastery in the workflows listed above I have placed lesson links throughout this chapter so that you can build these skills and be successful in this course.

## Pre-Course Skills & Setup

For the purpose of this course we will largely be using the following tools to access, pull, and explore data:

1. R & Rstudio
2. Git, GitHub, & Atom.io
3. Markdown & Rmarkdown

As such we will need to install and/or update these tools on your personal computer *before* our first day of class.  While we chose R for this course, nearly all of the packages and data are fully available and transferable to Python or other languages.  If you'd like to brush up on your R skills I highly recommend Data Carpentry Boostcamp's free [R for Reproducible Scientific Analysis](http://swcarpentry.github.io/r-novice-gapminder) course.

### Installing or Updating R
Please check your version of R.  You will need R 3.6.0+

How to check your version in R or RStudio if you already have it:
```
> version
               _                           
platform       x86_64-apple-darwin15.6.0   
arch           x86_64                      
os             darwin15.6.0                
system         x86_64, darwin15.6.0        
status                                     
major          3                           
minor          5.1                         
year           2018                        
month          07                          
day            02                          
svn rev        74947                       
language       R                           
version.string R version 3.5.1 (2018-07-02)
nickname       Feather Spray  
```
If you don't already have R or need to update it [do so here.](https://cran.rstudio.com/)


### Windows R/RStudio Setup
After you have downloaded R, run the .exe file that was just downloaded
Go to the [RStudio Download page](https://www.rstudio.com/products/rstudio/download/#download)
Under Installers select RStudio X.XX.XXX - e.g. Windows Vista/7/8/10
Double click the file to install it
Once R and RStudio are installed, click to open RStudio. If you don't get any error messages you are set. If there is an error message, you will need to re-install the program.

### Mac R/RStudio Setup

After you have downloaded R, double click on the file that was downloaded and R will install
Go to the [RStudio Download page](https://www.rstudio.com/products/rstudio/download/#download)
Under Installers select RStudio 1.2.1135 - Mac OS X XX.X (64-bit) to download it.
Once it's downloaded, double click the file to install it.
Once R and RStudio are installed, click to open RStudio. If you don't get any error messages you are set. If there is an error message, you will need to re-install the program.

## Linux R/RStudio Setup
R is available through most Linux package managers. You can download the binary files for your distribution from CRAN. Or you can use your package manager.
e.g. for Debian/Ubuntu
```
  run sudo apt-get install r-base
```
and for Fedora
```
  run sudo yum install R
```

To install RStudio, go to the [RStudio Download page](https://www.rstudio.com/products/rstudio/download/#download)
Under Installers select the version for your distribution.
Once it's downloaded, double click the file to install it
Once R and RStudio are installed, click to open RStudio. If you don't get any error messages you are set. If there is an error message, you will need to re-install the program.

### Install basic packages for this course
You can run the following script to make sure all the required packages are properly installed on your computer.



```r
# list of required packages
list.of.packages <- c(
  'data.table',
  'tidyverse',
  'jsonlite',
  'jpeg',
  'png',
  'raster',
  'rgdal',
  'rmarkdown', 
  'knitr'
)

# identify new (not installed) packages
new.packages <- list.of.packages[!(list.of.packages %in% installed.packages()[,"Package"])]

# install new (not installed) packages
if(length(new.packages)) 
  install.packages(new.packages, 
                   repos='http://cran.rstudio.com/')

# load all of the required libraries
sapply(list.of.packages, library, character.only = T)
```

**Note**: On some operating systems, you may need to install the Geospatial Data Abstraction Library (GDAL). More information about GDAL can be found from [here](https://trac.osgeo.org/gdal/wiki/DownloadingGdalBinaries).

## Installing and Setting up Git & Github on Your Machine

For this course you will need:
1. Git installed on your local machine
2. Very basic bash scripting
3. A linked GitHub account
4. To link RStudio to git via RStudio or Atom.io

As we will be using these skills constantly, they are a *pre-requisite* for this course.  If you don't yet have these skills it's okay!  You can learn everything that you need to know via the following freely available resources:

* [The Unix Shell](http://swcarpentry.github.io/shell-novice)

* [Version Control with Git](http://swcarpentry.github.io/git-novice)

* [Happy Git with R](https://happygitwithr.com/)

If you are learning these skills from scratch I estimate that you will need to devote ~4-6 hours to get set up and comfortable with the various workflows.  Also remember that I have code office hours every week and that Stack Exchange is your friend.

## Installing Atom

[Atom.io](https://atom.io/) is a powerful and useful text editor for the follwng reasons:

  1. It is langugae agnostic

  2. It fully integrates with git and github
    + You can use it to push/pull/resolve conflicts and write code all in one space.
  
## Linking RStudio to Git

[Happy Git with R](https://happygitwithr.com/rstudio-git-github.html) has a fantastic tutorial to help you link Rstudio-Git-Github on your local machine and push/pull from or to public repositories.




## How we will be Conducting this Course

At the end of each chapter you will find a set of **Exercises**.  At the end of the assigned chapter you will be expected to submit via BBLearn two files:
    1. An [RMarkdown file](https://rstudio.com/wp-content/uploads/2015/02/rmarkdown-cheatsheet.pdf) with the naming convention:
      LASTNAME_COURSECODE_Section#.Rmd,  and 
    2. A knitted .PDF with the same naming convention:
      LASTNAME_COURSECODE_Section#.pdf
  
To generate these files you have two options:

1. Click on the pencil and pad logo in the top of this text, copy the exercise section code, and drop it into your own .Rmd.
2. Git clone our [course Github Repository](https://github.com/katharynduffy/katharynduffy.github.io), navigate to the '_Exercises' folder, and use that .Rmd as a template.

*Note: Exercises submited in any other format, or those missing questions will not be graded*

To generate your .PDF to upload, in your RMarkdown file simply push the 'Knit' button at the top of your document.
