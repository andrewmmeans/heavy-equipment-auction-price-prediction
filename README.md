# Predict Heavy Equipment Auction Price
![alt text](https://github.com/andrewmmeans/heavy-equipment-auction-price-prediction/blob/master/images/wheel.jpeg)

## Background
Heavy equipment goes to auction, and nobody wants to over-pay. So we are trying to predict the sale price of a particular piece of heavy equipment at auction. 

## Data Acquisition 
The data is sourced from auction result postings and includes information on usage, equipment configurations, and a data dictionary to explain the columns in the data.

## Data Processing

The data was very messy with over 52 different features, so a very cutthroat process was used where most features were dropped. Features with high correlation to sales price and features that we had a hunch about were kept. We also got rid of all rows with NaN values. 


## Exploratory Data Analysis
We used a heatmap to get correlation data to sales price. 

![alt text](https://github.com/andrewmmeans/heavy-equipment-auction-price-prediction/blob/master/images/Screen%20Shot%202020-07-31%20at%205.46.02%20PM.png)

## Model
The features we included in the model were:
- Machine Hours Current Meter 
- Product group (type of equipment)
- Year Made
- Tire Size 

The model was built using linear regression and a single train test split. 


## Evaluation
The evaluation of our model was based on based on Root Mean Squared Log Error.
Which is computed as follows:

![Root Mean Squared Logarithmic Error](images/rmsle.png)

where *p<sub>i</sub>* are the predicted values (predicted auction sale prices) 
and *a<sub>i</sub>* are the actual values (the actual auction sale prices).

Our score was: RMSL = 0.597


## Another model

For this one, we worked with one product group, Backhoe Loaders.
We used more specific feature list: YearMade, Enclosure and Stick.
Our score turned out to be better: RMSL = 0.100





