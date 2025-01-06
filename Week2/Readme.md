First appropiate dataset(SuperStores Dataset) was preprocessed. 
Normalisation, encoding of categorial data,imputation to remove empty cells, 
datetime-series procesing are applied to make the data ready for the time-series forecasting.
Then ARIMA/SARIMA is applied , and the best values for all the variables are applied using the AIC values.
Appropiate graphs are plotted.
Then the Fb's Prophecy method is applied for forecasting, and the graph for forecasting is plotted accordingly.
For implementing Data of holidays, the builtin add_country_holidays can be used(used in the prophecy model), 
or another appropiate dataset of holidays can be imported and combined.The timedate functionality of used libraries already has access to the weekdays and weekends
Challenges- The ValueWarning, faced due to freq parameter not satified was no able to be rsolved in spite of setting 
the freq using .asfreq parameter in dataframe or inside the SARISA mmodel defination scheme.
The data,besides the sales and date values, can't be directly applied, 
rather techniques like RandomForest or Keras have to be implimented along with timeseries methods, 
application of which req more resources that couldn't be explored in time.
