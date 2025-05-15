# bambooImpute
mice imputations and data analysis for Japanese bamboo and forest datasets
# this code first extracts data froom a predefined dataset based on literature exracted variables. It then applies k-means clustering to vcreate climate zones, and factorises the data appropriate to observed management
# we then used the mice algorithm to impute aboveground, then belowground for bamboo and forest datasets
# next any remaining NA's are imputed in a combined above/belowground dataset
# any columns containing NA#s at this piint are discarded
# 10-fold cross-validation is then performed to ensure model stability
# variables which meet criteria set out in Forster et al. 2022 are retained for statistical analysis

# in the data analysis, the imputed dataframe is invoked and subjected to statistical analysis using Kruskal-Wallis, generalised least squares, and wilcoxen tests

# figures and tables are also produced where appropriate
