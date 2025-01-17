
# NanostringSkinPPGPaper

<!-- badges: start -->
<!-- badges: end -->

The goal of this repository is the house the reproducible code for the the Nanostring
Skin PPG paper. 


# Data
The AnalysisReport.Rmd contains the current analysis for the Nanostring data. The 
processed data containing the phenotype information, raw and standardizaed reads
is available on Cyverse at the link below. 

https://data.cyverse.org/dav-anon/iplant/projects/SkinPPG/H202SC24094550/Nanostring/Processed/StandardizedNanostringData.rds


# Data loading 
The AnalysisReport.Rmd uses HTTP access via WebDav to automattically load the processed
data from Cyverse into the R environment. An example of this code is below. 

```
# This is a link to the processed data on cyverse
data_path = data_path = "https://data.cyverse.org/dav-anon/iplant/projects/SkinPPG/H202SC24094550/Nanostring/Processed/StandardizedNanostringData.rds" 

# You may need to edit this code to update path
normalizedData <- readRDS(url(data_path))
```

# Download this repository
To download this repository and run the analysis, make sure you have git installed. 
For help installing git or using git with git hub, [here is a reference to help you
get started](https://docs.github.com/en/get-started/getting-started-with-git). If 
you have git set up, you can clone this repository with:

```
git clone https://github.com/JoelParkerUofA/NanostringSkinPPGPaper.git
```
Or you can download the zip file by clicking the green "code" button on the top 
right hand corner of the repository. 

