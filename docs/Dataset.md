### Dataset & Approach
The dataset used for our project can be found [here](https://ourworldindata.org/coronavirus/country/united-states?country=~USA).


Below is the Approcah we took for this project:

   * Data understanding and EDA
	 * Data type, data range constraints 
	 * Looking for missing data
	 * Looking for inconsistencies in data
	 * Visualizing the above to get a beteer insight in the uniformity or the inconsistencies
	 * Understanding and comapring distribution through histograms, CDF, PMF and KDE plots
	 * Visualizing relationshsips between the variables
	
   * Data Preparation
	 * Handling missing data with imputation or deletion (preferably imputation)
	 * Handling data types by converting some if needed
	 * Handling the scaling and normalizing of the data
	 * Dealing with pre-processing feature engineering: encoding, handling numerical and date variables
	 * Feature selection: 
		 * removing the redundancy, 
		 * checking correlation via a matrix and plot to understand which variables to select, 
		 * if necessary dimension reduction by PCA 

   * Machine Learning (Supervised)
	 * We will be approaching this project with supervised learning models to understand the effect of GDP and predict deaths

   * Evaluation
	 * Splitting the data into train and test set
	 * Scores, classification reports, confusion matrix to understand the accuracy of classification predictions
         * Exploring this with cross validation as well
	 * Tuning the hyperparameter and also planning to apply grid search for such hyper parameter tuning
