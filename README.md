
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


