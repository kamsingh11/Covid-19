# COVID-19
## Team Members

 - [Kamlesh Singh](https://github.com/kamsingh11)
 - [Mrunmayee Kulkarni](https://github.com/MrinmayeeKulkarni)
 - [Paul Atkins](https://github.com/patkins2)
 - [Andrew Lee](https://github.com/alee115)
 - [Pranjal](https://github.com/pranjal7842)

## Project Introduction

COVID-19 has been affecting every region of this world and this pandemic has taken the world by storm. This project focuses on the effects of pandemic based on age, region, GDP and such. The dataset obtained for this project is called  "the complete Our World in Data COVID-19 dataset" which is a collection of the COVID-19 data maintained by "[Our World In Data](https://ourworldindata.org/coronavirus)". This dataset is updated on a daily basis and includes variables such as confirmed cases, deaths, and testing, along with other potential variables.

## Research Question
We seek to understand how COVID-19 is affecting people of various ages, to predict the number of deaths and to determine the effect of GDP on pandemic response and vice versa.

## Relevant Domain Information
### Below are some links to more articles that relate to our research question:

 1. [The Cost of COVID-19: A Rough Estimate of the 2020 US GDP Impact](https://www.mercatus.org/publications/covid-19-policy-brief-series/cost-covid-19-rough-estimate-2020-us-gdp-impact)
 
This link is an interesting article breaking down data to explain how COVID has affected the GDP of the US. This article goes much further into the economic impact of COVID and does a great job of even breaking down industries. Our data breakdown will be much more broad with a global scope.

 2. [COVIDView: A Weekly Surveillance Summary of U.S. COVID-19 Activity](https://www.cdc.gov/coronavirus/2019-ncov/covid-data/covidview/index.html)
 
This article does an excellent job breaking down labs, hospitalizations, mortality, ethnicity and age. This article is also great because they do age adjustments on their data.

 3. [IMF: POLICY RESPONSES TO COVID-19](https://www.imf.org/en/Topics/imf-and-covid19/Policy-Responses-to-COVID-19)
 
This is not an article but a link to IMF's policy response tracker for Covid 19. It is very useful in understanding our research question as it lays down each country's history with this pandemic as well as their previous and current response and the way they are or have planned to reopen their economy.

 4. [Global Economic Effects of COVID-19](https://fas.org/sgp/crs/row/R46270.pdf)
 
This is a detailed report by Congressional Research Service gives a detailed insight about the economic effects of Covid 19 globally.With monthly economic developments laid out from March '20 to July '20.

## Data Sources
The dataset used for our project can be found [here](https://ourworldindata.org/coronavirus/country/united-states?country=~USA).

Approach (how you plan to address the research question):

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

   * Machine Learning (if applicable - supervised, unsupervised)
	* We will be approaching this project with supervised learning models to understand the effect of GDP and predict deaths

   * Evaluation
	* Splitting the data into train and test set
	* Scores, classification reports, confusion matrix to understand the accuracy of classification predictions
        * Exploring this with cross validation as well
	* Tuning the hyperparameter and also planning to apply grid search for such hyper parameter tuning

## Known Issues (problems with predictors, reporting, bias, etc.)
Upon initial evaluation of the data, there are several countries that do not report on all of the data attributes. 
This will require us to either fill large portions of missing data or omit large sections of the dataset. 

## Conclusion


