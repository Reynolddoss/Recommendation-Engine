# Recommendation-Engine
	AI powered recommendation system based on RFM score and clustering technique.
    • Recency (R) as days since last purchase: How many days ago was their last purchase? Deduct most recent purchase date from today to calculate the recency value. 1 day ago? 14 days ago? 500 days ago?
    • Frequency (F) as total number of transactions: How many times has the customer purchased from our store? For example, if someone placed 10 orders over a period of time, their frequency is 10.
    • Monetary (M) as total money spent: How many $$ (or whatever is your currency of calculation) has this customer spent? Simply total up the money from all transactions to get the M value.


# Prerequsites 
```
	* Python 3
	
```
# Libraries Used
	* Sklearn
	* Pandas

## Task:1(First Cluster)
1. Provided with a dataset of retail data as csv file. As a first part, using KMeans clustering to cluster the users into different segments based on RFM value. 
2. This will group the customers into different segments based on RFM score.
3. Retailer owner can create marketing campaign for specific target of customers satisfying a particular RFM value.

## Task:2(Sub Clusters)
1. Once this RFM based segmentation is done, Perform second level segmentation within each RFM segment. i.e. creating clusters within the segments using  socio-demographic attributes like age, gender. 
2. This helps to group like minded people or people having similar tastes and preferences. 
3. KMeans clustering is used to find similar customers having same taste and preferences within the segment. This is done by clustering of customers based on socio-demographic attributes.

## Task:3(Recommendation)
1. Identify the top most sold item within each cluster and recommend that item to customers who have not purchased the item. 



# NOTE
```
RFM based segmentation can’t be used to cluster like minded people. Eg:- Customers visited recently to a retail shop with high frequency in their visit with a  large monetary value may fall under same segment. But within the segment there will be people of different age, gender and other geospatial attributes.
```
