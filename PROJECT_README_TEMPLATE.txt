=== SDOH TOOLKIT — PROJECT README ===

Author:           [Your name]
Institution:      [Your institution]
Date completed:    2026-05-24 
Research question:[One sentence]

--- Analysis configuration ---
State:             il 
Geography:        County level
Outcome variable:  diabetes_pct 
Predictors:        poverty_rate, pct_bachelor_plus, uninsured_rate, pct_lila_tracts, social_associations 
Analysis label:    diabetes_sdoh_model 

--- Script run order ---
01_acs.R → 02_places.R → 03_svi_eji.R → 04_hrsa.R
→ 05_usda_nces_chr.R → 06_merge_all.R → 07_analysis.R

--- Data download dates ---
ACS 2020-2024:    [date]
CDC PLACES 2025:  [date]
SVI 2022:         [date]
EJI 2024:         [date]
HRSA AHRF 2024-25:[date]
USDA Atlas 2019:  [date]
CHR&R 2025:       [date]
NCES CCD 2024-25: [date]

--- Output files ---
Master CSV:    data/master/sdoh_ il _master.csv
Tableau CSV:   output/tableau/sdoh_ il _tableau.csv
Descriptive:   output/tables/01_descriptive_ diabetes_sdoh_model .csv
LM results:    output/tables/03_lm_results_ diabetes_sdoh_model .csv
Logit results: output/tables/04_logit_OR_ diabetes_sdoh_model .csv
Correlation:   output/figures/02_correlation_ diabetes_sdoh_model .png
Diagnostics:   output/figures/03_lm_diagnostics_ diabetes_sdoh_model .png

--- GitHub repository ---
Repository URL: [your GitHub URL]
Visibility:     Public

--- R environment ---
R version: 4 . 5.2 
OS: Windows 10 x64 

--- Package versions ---
tidycensus : 1.8.0 
tidyverse : 2.0.0 
haven : 2.5.5 
readxl : 1.5.0 
janitor : 2.2.1 
skimr : 2.2.2 
corrplot : 0.95 
car : 3.1.5 
broom : 1.0.13 
lmtest : 0.9.40 
ResourceSelection : 0.3.6 
sandwich : 3.1.1 
zipcodeR : 0.3.5 
