Firstly, the dataset is selected and preprocessing is done upon it.
Imputation is not helpful here, hence just remove those records.
The duplicate records are also removed.
In my opinion, there were two ways of customer segmentation, 
first that segments them on basis of how much they contribute to sales and how often they purchase.
the second segmentation is based on what type of products they buy.
The first type of segmentation would assist in formation of that type of marketing strategy that 
aims to keep loyal customers engaged
The second would assist in the decision of advertisement of which category of products should be the major target
to which type of customers.
K-means cluster techniques and dbscan is applied directly to the first segmentation as its bi-variate.
In order to apply unsupervised learning for the second segmentation strategy, first  
feature engineering using the description is done, keeping in mind to ignore adjectives, particularly colours.
I assumed that the most generic category for the item could be found in the last 2 words of the description(excluding the colors).
Then the extracted item categories are encoded using the dummy variables method.
For both the first and second segmentation strategy, min-max scaler is used as that seems to provide type of
normalising scaling appropiate for our model.
TSNE is then applied to convert the multivariate database to a bivariate numpy array.
Now similar to first segmentation, k-means clustering is applied.
Regarding DBSCAN, as applied in the first strategy, using divide-and-conquer like analogy(for each place after decimal, 
first checking the 5th place and then between either 1 and 5 or 5 and 9,then when we get it to be between x and x+1 digit, we go to the next decimal)
 to find the appropiate epsilon;
the appropiate epsilon should lie between 0.348954 and 0.348955, and the minimum samples are based on the scatter plot we draw in 
the k-means cluster method earlier.However it seems that DBSCAN is not an appropiate choice for this first segmentation strategy.   
