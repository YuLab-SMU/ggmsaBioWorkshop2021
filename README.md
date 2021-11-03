# ggmsa workshop

## Overview

The stacked alignment graphic that represents all individual sequences as rows and homologous residue positions as columns is used almost universally in the visualization of multiple sequence alignment (MSA). We present the R package ggmsa to extend MSA visualization method via integrating stacked MSAs and associated data. Sequence-related data sets such as secondary structures, genes locus, or phenotype are allowed to combining with MSA for exploring the sequence-structure-function relationship. And we developed and integrated multiple alignment visualization methods such as nucleotide difference plots, nucleotide similarity plots, and sequence bundles to exploring multifaceted sequence features from multiple perspectives. 

The workshop will be organized into two broad sections:

* Visually exploration of Conservation and Variation in MSAs    
* Visually exploration of MSAs' associations to phenotypes.

## Pre-requisites 

The course is aimed at PhD students, Master's students, and third & fourth year
undergraduate students. 
Some basic R knowledge is assumed - this is not an introduction to R course. 
If you are not familiar with the R statistical programming language it is
compulsory that you work through an introductory R course before you attend this workshop.

## _R_ packages used

The following key R packages will be used: 

* `ggmsa`
* `ggplot2`
* `phangorn`
* `ggtree`
* `Biostrings`
* `ggnewscale`
* `RColorBrewer`
* `dplyr`
* `gggenes`
* `readxl`


    
## Time outline

| Activity                                                        | Time |
|-----------------------------------------------------------------|------|
| Introduction                                                    | 10m  |
| 1.Visually exploration of Conservation and Variation in MSAs    | 30m  |
| 2.Visually exploration of MSAs' associations to phenotypes.     | 10m  |
| Q & A                                                           | 10m  |


## Workshop goals and objectives

### Learning goals

 - Learn how to perform ggmsa in R.
 - Understand the basic idea of MSA visualizations.

### Learning objectives

 - Get familiar with the package `ggmsa`
 - Perform different visualizations methods of MSA.

## Workshop package installation 

### Guide

This is necessary in order to reproduce the code shown in the workshop. 
The workshop is designed for R `4.1` and can be installed using one of the two ways below.

### Via Docker image

If you're familiar with [Docker](https://docs.docker.com/get-docker/) you could use the Docker image which has all the software pre-configured to the correct versions.

```
docker run -e PASSWORD=password -p 8787:8787 nyzhoulang/ggmsabioworkshop2021:latest
```

Once running, navigate to <http://localhost:8787/> and then login with
`Username:rstudio` and `Password:password`.

You should see the Rmarkdown file with all the workshop code which you can run.

### Via GitHub

Alternatively, you could install the workshop using the commands below in R `4.1`.

```
install.packages('remotes')

# Install workshop package
remotes::install_github("nyzhoulang/ggmsaBioWorkshop2021", build_vignettes = TRUE)

# To view vignettes
library(ggmsaBioWorkshop2021)
browseVignettes("ggmsaBioWorkshop2021")
```