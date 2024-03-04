[PROJECT]

Can you explain the price of electricity? [Ensemble Learning Course Project]

[DESCRIPTION]

The aim is to model the electricity price from weather, energy (commodities) and commercial data for two European countries - France and Germany. Let us stress that the problem here is to explain the electricity price with simultaneous variables and thus this is not a prediction problem.

[FEATURES]

Given 35 columns, sums of all renewable and non-renewable energies, weekday get by DAY_ID, DE_CONSUMPTION/DE_NET_IMPORT. Using Fourier Transform to transform data to detect frequency. 

[NOTEBOOKS USAGE] 

- Data_Inspection.ipynb
  Have a quick look at the variables and use classification to understand the variables. 
  Get the histogram of each variable, the result shows  that all variables are nomalized already and don't need further transformations. 
  Check correlation and quadratic relationship between variables. 

- Preprocess.ipynb
  Fill in null values of weather columns by averaging values of the day before and after. 
  Separate DE and FR data and variables. 
  Delete outliers using Three Gigma Rule. 
  Smoothing. 

- Model&FeatureEngineering_fr.ipynb
  Feature Engineering for FR data, and try 7 models on FR data. And choose 3 best-performed models: random forest, adaboost, knn.  

- Rf_Tuning_fr.ipynb
  Hyperparameter tuning for random forest. 

- Adaboost_Tuning_fr.ipynb
  Hyperparameter tuning for adaboost. 

- Knn_Tuning_fr.ipynb
  Hyperparameter tuning for knn. 

- Model&FeatureEngineering_de.ipynb
  Feature Engineering and PCA for DE data, and try the same 7 models on DE data. And choose 3 best-performed models: linear regression, svr, random forest. 

- SVR_Tuning_de.ipynb
  Hyperparameter tuning for svr. 

- Rf_Tuning_de.ipynb
  Hyperparameter tuning for random forest. 

- Test.ipynb
  Evaluation on test data. 
