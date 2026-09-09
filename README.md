# diet-microbiome-depression-ml
Analysis code for an MSc thesis on depression classification using dietary and gut microbiome features.

### Execution Order of the scripts

This project requires both Python and R. Please ensure you have installed the requirements for both environments before starting.

1. Pre-process the raw abundance file: 

bash
python dataset1_taxa_preprocessing.py

2. Check the correlation of diet variables:

bash
python dataset1_diet_correlation.py

3. Run feature selection on abundance data. Run ML models on remaining diet variables and selected taxonomic features.

bash
python dataset1_filtered_diet_ml_pipeline.py

4. Performance metrics and plots for the best-performing ML model

bash
Rscript dataset1_svm__plot.R

5. Visual plots for the important diet- and taxonomic-features.

bash
python dataset1_posthoc_diet_and_boxplots.py

6. Differential-abundance analysis by using ANCOM-BC2 on taxonomic features.

bash
Rscript dataset1_ancombc2_analysis.R
