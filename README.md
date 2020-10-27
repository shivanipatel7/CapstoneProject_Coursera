## CapstoneProject_Coursera

### Project Intro/Objective 
The purpose of this project is to cluster cities that have a significant amount of coronavirus cases based on the types of venues in that city 

### Methods Used 
* One hot encoding  
* K-means clustering 

### Technologies 
* Python 
* Kaggle 
* Folium 
* Forsquare API

### Project Description 
For each city with a significant amount of confirmed Coronavirus cases, Leverage the Forsqaure API to get all of the venues within a certain radius of the city. Using the top 15 venues for each city, group the cities into clusters to see if the types of venues can be used to create different clusters.  

Question: Can different cities within the United States with more than 275 Coronavirus cases be clustered into groups based on the types of venues in each city? 

### Data: 
Kaggle Coronavirus Time Series Dataset: https://www.kaggle.com/imdevskp/corona-virus-report 
<br>Forsqaure Places API: https://developer.foursquare.com/docs/api/venues/explore 

### Featured Notebooks: 
https://github.com/shivanipatel7/CapstoneProject_Coursera/blob/main/CoronaVirus%20Analysis%20with%20Forsquare%20API.ipynb

### Results: 
![alt text](https://github.com/shivanipatel7/CapstoneProject_Coursera/blob/main/results.png?raw=true)

### Analysis of Results: 
<br>The results provided above show that almost all areas have been assigned to cluster '2' and '1' (purple and blue). Because the k-means clustering is placing all the cities into 2 clusters, this may mean that the data contains outliers, the density spread of data points across the data space is different, and/or the data points follow non-convex shapes.

**Possible causes for this**
* Forsquare API limitation: venues returned within a certain radius by the Forsquare API are too similar across US cities. 
* Top Venues will always be similar: Top venues in most cities across the US will not vary(resturants, stores, pharmaticies etc). Venues are not the proper feature to find distinctions in different cities. 
* Clustering algorithm: K-means is not the best clustering algorithm to use to put the cities into different categories.

### Conclusion: 
Based on our findings, we must conclude that venues are not the best way to cluster corona-virus outbreak cities in the US as clustering cities based on venue categories resulted in overfitting. 
