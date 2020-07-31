# Predict Heavy Equipment Auction Price

## Background
Data on heavy equipment was used to try to predict the sale price of a particular piece of heavy equipment at auction. 

## Data Acquisition 
The data is sourced from auction result postings and includes information on usage, equipment configurations, and a data dictionary to explains the columns in the data.

## Data Processing

The data was very messy so a very cutthroat process was used where most features were dropped and the ones with high correlation to sales price was kept. 


## Exploratory Data Analysis
We used a heatmap to get correlation data to sales price. 

## Model
We built a model using linear regression and a single train test split. 


## Evaluation
The evaluation of our model was based on based on Root Mean Squared Log Error.
Which is computed as follows:

![Root Mean Squared Logarithmic Error](images/rmsle.png)

where *p<sub>i</sub>* are the predicted values (predicted auction sale prices) 
and *a<sub>i</sub>* are the actual values (the actual auction sale prices).

