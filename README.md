# Predict Heavy Equipment Auction Price
![alt text](https://github.com/andrewmmeans/heavy-equipment-auction-price-prediction/blob/master/images/wheel.jpeg)

## Background
Heavy equipment goes to auction, and nobody wants to over-pay. So we are trying to predict the sale price of a particular piece of heavy equipment at auction. 

## Data Acquisition 
The data is sourced from auction result postings and includes information on usage, equipment configurations, and a data dictionary to explain the columns in the data.

## Data Processing

The data was very messy so a very cutthroat process was used where most features were dropped. Features with high correlation to sales price and features that we had a hunch about were kept. They include:
- Machine Hours Current Meter 
- Product group (type of equipment)
- Year Made
- Tire Size 


## Exploratory Data Analysis
We used a heatmap to get correlation data to sales price. 

![alt text](https://github.com/andrewmmeans/heavy-equipment-auction-price-prediction/blob/master/images/Screen%20Shot%202020-07-31%20at%205.46.02%20PM.png)

## Model
We built a model using linear regression and a single train test split. 


## Evaluation
The evaluation of our model was based on based on Root Mean Squared Log Error.
Which is computed as follows:

![Root Mean Squared Logarithmic Error](images/rmsle.png)

where *p<sub>i</sub>* are the predicted values (predicted auction sale prices) 
and *a<sub>i</sub>* are the actual values (the actual auction sale prices).

