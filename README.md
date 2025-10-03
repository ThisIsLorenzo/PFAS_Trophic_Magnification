# PFAS Trophic Magnification: A Meta-Analysis 
## Study Overview
This repository contains all data, code, and analysis materials for the research study: "*A meta-analysis reveals PFAS concentrations double with each trophic level*".

Our research demonstrates significant biomagnification of per- and polyfluoroalkyl substances (PFAS) through food webs, with concentrations doubling at each trophic level.

You can find the Preprint at the following link: [EcoEvoRxiv](https://ecoevorxiv.org/repository/view/8548/)

## Repository Structure
### Analysis scripts (`/R`)
Contains R markdown files (`.Rmd`) with corresponding HTML outputs documenting the analysis.
-  `/R/Analysis_code.Rmd`: General analysis code. It hosts the analyses conducted to generate model results and plots.
-  `/R/random_splitting.Rmd`: We utilised this code to evenly split the bibliographic records among reviewers during the literature search.
-  `/R/deduplication.Rmd`: We utilised this code to remove duplicates from the bibliographic records extracted from Rayyan.
-  `/R/Slope_calculations.Rmd`: The file contains trophic magnification slope calculations using data manually extracted from plots (see *Data extraction from plots*). A user-friendly and easy-to-read version of this file is available at `/R/Slope_calculations.html`.
-  `/R/TMFs_comparison.Rmd`: In this file, we report a validation analysis of trophic magnification slopes calculated against the reported values by the included studies in the meta-analysis. A user-friendly and easy-to-read version of this file is available at `/R/TMFs_comparison.html`.
-  `/R/Model_validation.Rmd`: We utilised this code to validate our subgroup-correlated effects meta-regression model. A user-friendly and easy-to-read version of this file is available at `/R/Model_validation.html`.
  
### Data files (`/data`)
Houses all datasets in CSV format used in the analysis.
-  `/data/study_data.csv`: Raw data related to characteristics of the included studies in the meta-analysis (Data S1). Data were extracted from the included studies.
-  `/data/fw_data.csv`: Raw data related to parameters of food webs (Data S2). Data were extracted from the included studies.
-  `/data/PFAS_data.csv`: Raw data related to PFAS analytes (Data S3). Data were extracted from the included studies.
-  `/data/TMF_data.csv`: Quantitative datasets used for effect size calculations (Data S4). Data were extracted from the included studies.
-  `/data/RoB_data.csv`: Study validity assessment results (Data S5).
-  `/data/deduplication/from_Rayyan_combined.csv`: Bibliographic records extracted from Rayyan.
-  `/data/deduplication/deduplicated.bib`: Bibliographic records extracted from Rayyan after undergoing deduplication in R.
-  `/data/splitting/deduplicated_R+Rayyan.bib`: Bibliographic records ready for screening. The records were deduplicated in R and Rayyan.
-  `/data/splitting/split1.bib`: One sixth of the bibliographic records assigned to the first of the six authors conducting literature screening.
-  `/data/splitting/split2.bib`: One sixth of the bibliographic records assigned to the second of the six authors conducting literature screening.
-  `/data/splitting/split3.bib`: One sixth of the bibliographic records assigned to the third of the six authors conducting literature screening.
-  `/data/splitting/split4.bib`: One sixth of the bibliographic records assigned to the fourth of the six authors conducting literature screening.
-  `/data/splitting/split5.bib`: One sixth of the bibliographic records assigned to the fifth of the six authors conducting literature screening.
-  `/data/splitting/split6.bib`: One sixth of the bibliographic records assigned to the sixth of the six authors conducting literature screening.

### R generated data (`/Rdata`)
Includes all data generated through analysis.
### Statistical models (`/Rmodels`)
Contains saved model objects (`.RData` files) from statistical analyses, allowing for reproducibility and further exploration without recomputation.
### Visualisations (`/figs`)
Includes all main and supplementary figures.
### Data extraction from plots (`/metaDigitise/Raw_data.csv`)
Contains data extracted from published literature using the metaDigitise software.
### Project file
`PFAS_Trophic_Magnification.Rproj` - RStudio project file for convenient access to the complete analysis environment.


Repository curated by *Lorenzo Ricolfi*
