# bambooImpute
# Mice imputations and data analysis for Japanese bamboo and forest datasets
#Contact: danforster.grassland@hotmail.com
# It consists of two scripts executable in R. 'Bamboo forest imputations' performs data processing and imputation. 'Data analysis for bamboo forests' performns statistical analysis on the imputed data.

#The scripts both contain generic filepaths and data variable names. These should be tailored to your dataset prior to use.

#1
# They extract data froom a predefined dataset based on literature exracted variables. It then applies k-means clustering to create climate zones, and appropriately factorises the data to observed managements and other factors.

# It then employs the mice algorithm and a random forests (rf) method to impute first aboveground, then belowground & GHG related variables for bamboo and forest datasets.

# Any remaining NA's are then imputed in a combined above/belowground dataset.

# Columns containing NA's at this point are discarded.

# 10-fold cross-validation is then performed to ensure model stability.

# Variables which meet criteria set out in Forster et al. 2022 are retained for statistical analysis and passed to the second script.

#2
# In the data analysis, the imputed dataframe is invoked and subjected to statistical analysis using Kruskal-Wallis, generalised least squares, and wilcoxen tests.

# Figures and tables are also produced where appropriate


