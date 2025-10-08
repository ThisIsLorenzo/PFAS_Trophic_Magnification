# PFAS Trophic Magnification: A Meta-Analysis 
## Study Overview
This repository contains all data, code, and analysis materials for the research study: "*Unravelling the magnitude and drivers of PFAS trophic magnification*".

You can find the Preprint at the following link: [EcoEvoRxiv](https://ecoevorxiv.org/repository/view/8548/)

Repository created and curated by *Lorenzo Ricolfi*

## Repository Structure

### Project file
`PFAS_Trophic_Magnification.Rproj` - RStudio project file for convenient access to the complete analysis environment.

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

### Analysis scripts (`/R`)
Contains R markdown files (`.Rmd`) with corresponding HTML outputs documenting the analysis.
-  `/R/Analysis_code.Rmd`: General analysis code. It hosts the analyses conducted to generate model results and plots.
-  `/R/random_splitting.Rmd`: We utilised this code to evenly split the bibliographic records among reviewers during the literature search.
-  `/R/deduplication.Rmd`: We utilised this code to remove duplicates from the bibliographic records extracted from Rayyan.
-  `/R/Slope_calculations.Rmd`: The file contains trophic magnification slope calculations using data manually extracted from plots (see *Data extraction from plots*). A user-friendly and easy-to-read version of this file is available at `/R/Slope_calculations.html`.
-  `/R/TMFs_comparison.Rmd`: In this file, we report a validation analysis of trophic magnification slopes calculated against the reported values by the included studies in the meta-analysis. A user-friendly and easy-to-read version of this file is available at `/R/TMFs_comparison.html`.
-  `/R/Model_validation.Rmd`: We utilised this code to validate our subgroup-correlated effects meta-regression model. A user-friendly and easy-to-read version of this file is available at `/R/Model_validation.html`.

### R-generated data (`/Rdata`)
Includes all data generated through analysis.
-  `/Rdata/fig1_data.csv`: Source data for figure 1
-  `/Rdata/fig2A_data.csv`: Source data for figure 2 panel A
-  `/Rdata/fig2B_data.csv`: Source data for figure 2 panel B
-  `/Rdata/fig3A_data.csv`: Source data for figure 3 panel A
-  `/Rdata/fig3B_data.csv`: Source data for figure 3 panel B
-  `/Rdata/fig3C_data.csv`: Source data for figure 3 panel C
-  `/Rdata/fig3D_data.csv`: Source data for figure 3 panel D
-  `/Rdata/fig4A_data.csv`: Source data for figure 4 panel A
-  `/Rdata/fig4B_data.csv`: Source data for figure 4 panel B
-  `/Rdata/fig4C_data.csv`: Source data for figure 4 panel C
-  `/Rdata/fig5A_data.csv`: Source data for figure 5 panel A
-  `/Rdata/fig5B_data.csv`: Source data for figure 5 panel B
-  `/Rdata/fig5C_data.csv`: Source data for figure 5 panel C
-  `/Rdata/fig5D_data.csv`: Source data for figure 5 panel D
-  `/Rdata/fig5E_data.csv`: Source data for figure 5 panel E
-  `/Rdata/fig5F_data.csv`: Source data for figure 5 panel F
-  `/Rdata/aic_weights.csv`: Model-selection summaries
-  `/Rdata/TMF_data2.csv`: Modified dataset (see analysis code)
-  `/Rdata/TMF_data3.csv`: Modified dataset (see analysis code)

### Statistical models (`/Rmodels`)
Contains saved meta-analytic mixed-effects model objects (`.RData` files) from statistical analyses, allowing for reproducibility and further exploration without recomputation. 
- `/Rmodels/breath_model.RData`
- `/Rmodels/breath_model_int.RData`
- `/Rmodels/bt_fw_model.RData`
- `/Rmodels/ccl_model.RData`
- `/Rmodels/class_model.RData`
- `/Rmodels/eco_aq_model.RData`
- `/Rmodels/eco_model.RData`
- `/Rmodels/full_model.RData`
- `/Rmodels/fw_length_model.RData`
- `/Rmodels/lat_model.RData`
- `/Rmodels/location_model.RData`
- `/Rmodels/MLMR_mod_year.c.RData`
- `/Rmodels/mod.RData`
- `/Rmodels/mod_candidate.RData`
- `/Rmodels/mod_chem.RData`
- `/Rmodels/mod_chem_contr.RData`
- `/Rmodels/mod_chem1.RData`
- `/Rmodels/mod_chem2.RData`
- `/Rmodels/mod_chem3.RData`
- `/Rmodels/mod_ecogroup.RData`
- `/Rmodels/mod_RoB.RData`
- `/Rmodels/mod_se.RData`
- `/Rmodels/n_species_model.RData`
- `/Rmodels/norm_model.RData`
- `/Rmodels/norm_model2.RData`
- `/Rmodels/p_ccl_model.RData`
- `/Rmodels/regulation_model.RData`
- `/Rmodels/rv_model.RData`
- `/Rmodels/sample_model.RData`
- `/Rmodels/tef_model.RData`
- `/Rmodels/TL_highest_model.RData`
- `/Rmodels/TL_lowest_model.RData`
- `/Rmodels/undetected_model.RData`

### Visualisations (`/figs`)
Includes all main and supplementary figures.
- `/figs/fig1.pdf`: World map showing the geographical distribution of the 119 food webs included in the meta-analysis.
- `/figs/fig2.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS) in food webs. The light and dark green shields were added outside the R environment.
- `/figs/fig3.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by sample type (A), concentration determination method (B), trophic enrichment factor (C), and treatment strategy of undetected values (D).
- `/figs/fig4.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by food webs of exclusively water breathing organisms versus mixed breathing types (A), food webs with either air breathing or water breathing top predators (B), and PFAS chemical class (C).
- `/figs/fig5.pdf`: The relationship between trophic magnification of per- and polyfluoroalkyl substances (PFAS) and food webs’ latitude (A), trophic position of the food web’s baseline organism (B), trophic position of the food web’s top predator (C), the number of trophic levels in the food web (D), PFAS carbon chain length (E), and publication year of the included studies in the meta-analysis (F).
- `/figs/supplements/figS1.pdf`: Trophic magnification of per- and polyfluoroalkyl substances (PFAS) in aquatic and terrestrial food webs.
- `/figs/supplements/figS2.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by geographic location of food webs.
- `/figs/supplements/figS3.pdf`: The relationship between trophic magnification of per- and polyfluoroalkyl substances (PFAS) and perfluoroalkyl chain length.
- `/figs/supplements/figS4.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by broad ecosystem type (terrestrial vs aquatic).
- `/figs/supplements/figS5.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS) in aquatic ecosystems, stratified by ecosystem type (marine vs freshwater).
- `/figs/supplements/figS6.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS) in food webs.
- `/figs/supplements/figS7.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by sample type.
- `/figs/supplements/figS8.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by concentration determination method.
- `/figs/supplements/figS9.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by trophic enrichment factor.
- `/figs/supplements/figS10.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by treatment strategy of undetected values.
- `/figs/supplements/figS11.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by food webs of exclusively water breathing organisms versus mixed breathing types.
- `/figs/supplements/figS12.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by food webs with either air breathing or water breathing top predators.
- `/figs/supplements/figS13.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by PFAS chemical class.
- `/figs/supplements/figS14.pdf`: Trophic magnification factor (TMF) of per- and polyfluoroalkyl substances (PFAS), stratified by chemicals’ international regulation status.
- `/figs/supplements/figS15.pdf`: Alluvial plot of the overlap among the three categorical variables included in the full model.
- `/figs/supplements/figS16.pdf`: Relative importance of tested moderator variables based on Akaike weights, calculated from the Akaike Information Criterion (AIC).
- `/figs/supplements/figS17.pdf`: Funnel plot for visual inspection of studies’ precision.
- `/figs/supplements/figS18.pdf`: Publication bias test.
- `/figs/supplements/figS19.pdf`: Forest plot illustrating the results of leave-one-out sensitivity analyses.
- `/figs/supplements/figS20.pdf`: Model validation and profile likelihood for the 17 PFAS included in the subgroup-correlated effects model.
- `/figs/supplements/figS21.pdf`: Overall TMF after filtering out studies flagged by the study validity assessment.
- `/figs/supplements/figS22.pdf`: Search and screening flow PRISMA diagram.
- `/figs/supplements/figS23.pdf`: Diagram illustrating the structure of the relational database of the extracted data.
  
### Data extraction from plots (`/metaDigitise/Raw_data.csv`)
Contains data extracted from plots of published literature using the metaDigitise software.
- `/metaDigitise/Raw_data.csv`: Contains data extracted from plots of published literature using the metaDigitise software.
- `/metaDigitise/caldat`: Software-related files.
- `/metaDigitise/figures`: Figures from the literature which were used to extract data using the metaDigitise software.
