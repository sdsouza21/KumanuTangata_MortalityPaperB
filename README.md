# KumanuTangata_MortalityPaperB
This repository contains code files for manuscript titled "Addressing Healthy Worker Effects in the Mortality of Former New Zealand First-Class Rugby Players: Career Length, Highest Playing Level, and Position". This is Paper B of two companion papers currently in preparation. The repository for Paper A is available at https://github.com/sdsouza21/KumanuTangata_MortalityPaperA.
# Project Abstract
**Objective:** To assess healthy worker effects on mortality in former first-class male rugby players, using internal (career length, level played, position) and external (general population) comparison groups.

**Design:** Nationwide retrospective cohort study. 

**Setting:** New Zealand. 

**Participants:** 12,861 first-class male rugby players (active 1950–2000) and 2,394,342 general population males, weighted to match the player group for birth year, overseas-born status, and ethnicity.

**Main outcome measures:** All-cause mortality and cause-specific mortality (including cancer, cardiovascular, respiratory, metabolic, and neurodegenerative diseases) from mortality records between 1988 to 2020. 

**Methods::** Cox models compared mortality between player groups and with the general population.

**Results:** Longer careers were associated with higher neurodegenerative (≥6 vs 1 year: 1.42; 1.02 to 1.99) and lower respiratory disease mortality (0.56; 0.38 to 0.83). International/professional players had lower respiratory disease mortality (0.18; 0.04 to 0.70) than the general population, whereas provincial/amateur players had lower all-cause (0.92; 0.89 to 0.95), respiratory (0.59; 0.51 to 0.69) and metabolic (0.65; 0.53 to 0.80), but higher neurodegenerative disease mortality (1.27; 1.11 to 1.45). Forwards had higher all-cause mortality (HR 1.15; 95% CI 1.07 to 1.24), cardiovascular mortality (1.18; 1.03 to 1.35), and metabolic mortality rates (1.64; 1.03 to 2.60) than backs. Compared to the general population, both positional groups had lower respiratory disease mortality (forwards, 0.55; 0.42 to 0.71; backs, 0.59; 0.48 to 0.73) and higher neurodegenerative disease mortality (forwards, 1.29; 1.02 to 1.63; backs, 1.37; 1.14 to 1.64).

**Conclusions:** Former rugby players exhibit a complex mortality profile, with lower mortality for many causes versus the general population. This protective effect increases with career length, likely associated with the high fitness levels required for selection (i.e., healthy worker effect). However, this masks a significant sport-related risk: longer careers and higher levels of play are linked to increased neurodegenerative disease mortality, which underscore the need for ongoing health surveillance and targeted strategies to manage neurodegenerative disease risks.

# Statistical analyses
Data management was performed using SAS Enterprise Guide version 8.3, statistical modelling with Stata version 16.1, descriptive statistics with Microsoft Excel 2024, and charts were generated using Pandas, Numpy, and Matplotlib libraries in Python 3.12.

Cox proportional hazards models were used to compare relative mortality rates between levels of player groups and those of the general population. For comparisons between player groups and the general population we used direct standardisation for birth year (grouped into 5-year bands from 1920–24 to 1980–84), ethnicity (European, Māori, Pacific Island, and Other [combining Asian, Middle Eastern, Latin American, African, and other ethnicities]), and overseas-born (NZ-born, overseas) differences between rugby players and the general population. The direct standardisation method accounts for differences between players and the general population, but not for differences between player groups (e.g., by years played, position, etc.). Thus, for within-player cohort comparisons, covariate adjustment for birth year bands, ethnicity, and NZ-born status was used to account for differences between the groups on these factors. 

Most models did not meet the proportional hazards assumption. Given the large number of models, and to maintain parsimonious interpretation, hazard ratios (HR) should be interpreted as the average difference in rates of death between the groups across the follow-up period. It is important to acknowledge that this does not allow us to draw conclusion on time-varying risks; however, these are presented in our companion paper for overall cohort comparisons. Follow-up of mortality outcomes began from age 30, with right censoring for emigration, death, or the end of the study period (December 2020). For each cause-specific mortality analysis, participants were also right censored if their death was from other causes. The absolute risk difference between cohorts for each cause was reported per 1000 individuals. 

# Table of contents
1.Addressing Healthy Worker Effects in the Mortality of Former New Zealand First-Class Rugby Players_codefile.txt 

# Acknowledgements and authors
**Acknowledgements**
This work was supported by World Rugby Limited and the New Zealand Rugby Foundation [grant number G-2004-00963]. World Rugby obtained an independent, external review of the project plan prior to funding. The study funders had no role in study conception or design; data collection, analysis, and interpretation; and manuscript preparation and submission.  
We thank Statistics New Zealand and their staff for access to the Integrated Data Infrastructure and timely review of outputs. We also acknowledge the Public Policy Institute at the University of Auckland for access to their Statistics New Zealand Datalab, and Clive Akers for his collation of player records in the New Zealand Rugby Register. 

**Manuscript authors**
- Kenneth L. Quarrie, PhD 
- Chao Li, PhD 
- Barry J. Milne, PhD 
- Francesca Anns, BA(Hons) 
- Andrew Gardner, PhD 
- Ian Murphy, MB ChB 
- Evert Verhagen, PhD 
- Craig Wright, BSc 
- Susan M. B. Morton, PhD 
- Thomas Lumley, PhD 
- Lynette Tippett, PhD 
- John W. Orchard, MD, PhD 
- Joshua P. McGeown, PhD 
- Stephanie D’Souza, PhD

**Code authors**
- Kenneth L. Quarrie, PhD 
- Chao Li, PhD 
- Barry J. Milne, PhD
- Stephanie D’Souza, PhD

# Stats NZ Disclaimer
These results are not official statistics. They have been created for research purposes from the Integrated Data Infrastructure (IDI) which is carefully managed by Statistics New Zealand. For more information about the IDI please visit https://www.stats.govt.nz/integrated-data/.  
