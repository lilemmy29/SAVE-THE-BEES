# Save The Bees: Analysis of Honey Bee Colony Loss
This repository contains an analysis of factors contributing to the loss of honey bee colonies in the United States from 2015 to 2022. The data used in this study were collected by the USDA and curated into a manageable dataset for Exploratory Data Analysis (EDA) and predictions.


 ## Dataset
The dataset used in this study is available on Kaggle under the name "Save The Bees". You can access it here.

The dataset includes the following columns:

state: State within the USA. Note, "other" is a collection of states for privacy reasons. And the "United States" state is the average across all states.
num_colonies: Number of honey bee colonies.
max_colonies: Max number of honey bee colonies for that quarter.
lost_colonies: Number of colonies that were lost during that quarter.
percent_lost: Percentage of honey bee colonies lost during that quarter.
renovated_colonies: Colonies that were 'requeened' or received new bees.
percent_renovated: Percentage of honey bee colonies that were renovated.
quarter: Q1 is Jan to March, Q2 is April to June, Q3 is July to September, and Q4 is October to December.
year: Year between 2015 and 2022.
varroa_mites: Percentage of colonies affected by a species of mite that affects honey bee populations.
other_pests_and_parasites: Percentage of colonies affected by a collection of other harmful critters.
diseases: Percentage of colonies affected by certain diseases.
pesticides: Percentage of colonies affected by the use of certain pesticides.
other: Percentage of colonies affected by an unlisted cause.
unknown: Percentage of colonies affected by an unknown cause.


 ## Model
The model used in this study is a RandomForestClassifier. This is an ensemble method, meaning it combines predictions from multiple models. Each of the smaller models in the random forest ensemble is a decision tree, and predictions are made by calculating the prediction for each decision tree, then taking the most popular result.


 ## Key Findings
The analysis revealed that diseases have a significant impact on lost colonies. However, the impact of parasites such as Varroa Mites and other pests was not statistically significant based on the model.


 ## Future Directions
While the model did not directly include a variable for climate change, it's important to note that climate change could indirectly affect some of the variables in the model. For instance, climate change could potentially influence the prevalence of pests, parasites, and diseases. Future research should consider including direct measures of climate change to further elucidate its impact on bee colonies.

 ## Code
The code in this repository is written in Python and uses the statsmodels library to perform the OLS regression analysis.
