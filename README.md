# Temporal and environmental factors interact with rootstock genotype to shape leaf elemental composition in grafted grapevines 

This repository containts the Jupyter Notebooks used for the analysis of data in the manuscript currently hosted at: .

## Metadata Generation

`01. metadata_construction.ipynb` is a python notebook used to assign appropriate metadata to the sample names. 

## Imputation of Missing Values
`02.1. filter_for_KNN.ipynb` is an R notebook used to remove samples with outlier values prior to KNN fitting. `02.2. objectively_determine_k_50_30.ipynb` is a python notebook used for the imputation of missing data using KNN. `02.3. objectively_determine_k_plot.ipynb` is an R notebook used for plotting the results of the imputation. 

## Machine Learning
`03.1. clean_data_for_rf.ipynb` is an R script that merges the metadata on to the imputed data set for machine learning. `03.2. random_forest.ipynb` is a Python notebook for the machine learning component of the study. `03.3. random_forest_yearbypheno.ipynb` is an additional python notebook to fit a random forest to the year by phenology interaction which was missed in the larger script. `03.4. generate_confusion_matrices.ipynb` is a python notebook to plot the results from the maching learning portion of the study. 

## Linear Mixed Models
`04.1. LDA_ionomics.ipynb` is an R notebook used to inform linear model parameterization through LDA. `04.2. 1719_test_lmer.ipynb` is the R notebook used to fit the parameterized linear models and generate all subsequence plots. 

## Environmental Analysis
`05. 1719_weather_vineid.ipynb` is an R notebook used for the analysis of elemental composition as it varies with environmental variation and all subsequent plots. 

## License 

All scripts are provided for free: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
