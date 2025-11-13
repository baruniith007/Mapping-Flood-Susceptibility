Floods are devastating natural disasters that affect millions of people each year. To mitigate these impacts, it is crucial for policymakers and planners to identify areas that are prone to flooding. This enables targeted investments and the development of effective risk management strategies. Flood susceptibility mapping plays a key role in pinpointing these vulnerable regions.
In this article, we will develop a flood susceptibility map using two machine learning models: the Random Forest Classifier and the MLP Classifier.

The process is organized into five key steps:

Exploratory Data Analysis: We begin by examining the dataset through summary statistics, correlation analysis, and checking for missing values.
Feature Engineering: We employ the Sequential Feature Selection method to refine the feature set.
Model Development: With optimal features selected, we proceed to tune the hyperparameters of our models, followed by training and testing. We assess model performance using ROC_AUC plots and statistics derived from the confusion matrix.
Interpretability of the Models: To understand the influence of various features, we generate partial dependence plots and permutation feature importance plots.
Flood Susceptibility Mapping: After training and testing the models, we use the probabilistic outputs from model.predict_proba(features) to create a preliminary flood susceptibility map. This map is further refined using the Inverse Distance Weighting (IDW) technique in GIS and classified into five categories: very low, low, moderate, high, and very high.
This approach aims to provide a comprehensive tool for flood susceptibility assessment, aiding decision-makers in their efforts to safeguard vulnerable communities.

Study Area:
Two Flood Prone districts of Assam, India were selected for this project: Dhemaji & Kamrup Metro.

Data used:
Flood conditioning Factors: Twelve Flood Conditioning Factors were selected namely — Distance to River [DR] (m), Drainage Density [DD], DEM (m), slope, flow Accumulation [FA], MNDWI, NDBI, NDMI, NDVI, TWI, Average Daily Precipitation [Precip] (mm/hr.), and Curve Number [CN].
Flood Inventory: 1000 data points were collected from each map. 500 from flooded locations, 500 from non-flooded location.

