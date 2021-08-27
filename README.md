# Brief Portfolio for application of Data Analyst

The folders contain jupyter notebooks of Data analysis I have personally completed or Group work by me. 

Each of the notebook are written in Python3 however all initial datasets have not been included as I don't own this information

## ETL directory
This contains link to another Github repository that shows a group project that I contributed.  It shows use of ETL concept and tools such as SQL.

This was a  self-devised project to take information from two websites to compare countries average income against  countries level of happiness and record these is customer SQL database and draw conclusions.

## Regression 
The regression folder demonstrate example of both a Linear and Logistic regression based on real world data

The Client request to review FTE cost for employees at all Australian Universities over a 20 year period. They requested a regression prediction to make conclusion about future of the FTE cost. 

Initial EDA work was to generate custom groups requested by the client.  We then plotted some these groups to understand the distribution over time.  We then applied annual Medians and review the in average income overtime. 

Difficulties was the dataset was it was very heavily weighed toward the higher volume of lower income groups.  While the smaller higher income groups trends were masked.  Ultimately the Linear or Logistic regression did not prove useful.  It was agreed that changes to the groupings and the features would need to take place first.


## Predictive Models 
There are two directories showing models I have produced.  

### Supervised 
Random Forest directory hold notebook that has utilised a Random Forrest Regression Tree

Analytics Company reviewing ambulance usage in a Australian state by LGAs.  Dataset included number of calls, severity of calls, reason for call, socio-economic background each caller. 

The request produce model that would predict ambulance usage in a given LGA.  So the socio-economic features of a LGA could be altered for future predicted usage.

The was a significant amount of co-linearity and multilinear regression did not yield meaningful outcome. I decided to use a Random Forrest Regressor. It produced a model 
with a variance of predicted calls to actual of 0.04% show the last graph of r-forrest-regres.ipynb.  The green dots are predicted and line shows actual.  

Difficulties are the model was likely overfitted, as the model was based only 12 months.  I believe the model would have benefited from information long term information.

### Unsupervised

Unsupervised directory contains a K-mean model that was used to enrich and existing data and prediction engine.  

This was a self devised group project to create a functions web app that predicted a Beer based on you taste preference.  The full JS code etc has not been include here just notebook relating to the model. 

The goal was make predictor would able to pick 3 beers across different styles. Not just recommend like for like.  For example you might select strong heavy Ale and the predictor might recommend you a stout have some similar tastes.  We  scraped a beer review website as well as beer taste profile website and combined these into one dataset.  We wanted to then enrich our dataset machine learning. ML to create a new feature where the model clustered flavours.  Then finally use a cosine-similarity use the enrich information for the final prediction. 

Notebook shows the construction of K-mean cluster model to produce beer classes.  The cluster was optimised with K-mean++ initialisation.  Two approaches we trialled to input the information.  Firstly via normal dataframe next the dataframe was converted to a vector by beer.  Based on silhouette score, inertia and distortion testing the first approach provided the most consistent clusters. 

Difficulties was weighting of the dataset as there were a significant amount of common styles like ales reviewed than less popular artisan beers.  The model and predictor could have been adjusted mitigate this but the was not sufficient time to complete the project. 


![image](https://user-images.githubusercontent.com/3102930/131073030-a6e87c6f-813a-482d-911e-b262ae66ad86.png)
