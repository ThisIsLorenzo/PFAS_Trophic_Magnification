# PFAS Trophic Magnification: A Meta-Analysis 
## Study Overview
This repository contains all data, code, and analysis materials for the research study: "*A meta-analysis reveals PFAS concentrations double with each trophic level*".
Our research demonstrates significant biomagnification of per- and polyfluoroalkyl substances (PFAS) through food webs, with concentrations doubling at each trophic level.
## Repository Structure
### Analysis scripts (`/R`)
Contains R markdown files (`.Rmd`) with corresponding HTML outputs documenting the analysis.
-  `/R/Analysis_code.Rmd`: General analysis code.
-  `/R/Slope_calculations.Rmd`: The file contains trophic magnification slope calculations using data manually extracted from plots (see *Data extraction from plots*)
-  `/R/random_splitting.Rmd`: We utilised this code to evenly split the bibliographic records among reviewers during the literature search.
-  `/R/TMFs_comparison.Rmd`: In this file, we report a validation analysis of trophic magnification slopes calculated against the reported values by the included studies in the meta-analysis.
### Data files (`/data`)
Houses all datasets in CSV format used in the analysis.
-  `/data/study_data.csv`
-  `/data/fw_data.csv`
-  `/data/PFAS_data.csv`
-  `/data/TMF_data.csv`
-  `/data/RoB_data.csv`
### R generated data (`/Rdata`)
Includes all data generated through analysis.
### Statistical models (`/Rmodels`)
Contains saved model objects (`.RData` files) from statistical analyses, allowing for reproducibility and further exploration without recomputation.
### Visualisations (`/figs`)
Includes all figures generated for the manuscript and supplementary materials in PNG format.
### Data extraction from plots (`/metaDigitise/Raw_data.csv`)
Contains data extracted from published literature using the metaDigitise software.
### Project file
`PFAS_Trophic_Magnification.Rproj` - RStudio project file for convenient access to the complete analysis environment.
