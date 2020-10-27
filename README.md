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

Question: Can different cities within the United States with more than 275 Coronavirus cases be clustered into groups based on the types of venues in each city? Is there any relationship between the average number of cases in a city and the cluster the city is assigned to? 

### Data: 
Kaggle Coronavirus Time Series Dataset: https://www.kaggle.com/imdevskp/corona-virus-report 
<br>Forsqaure Places API: https://developer.foursquare.com/docs/api/venues/explore 

### Featured Notebooks: 
https://github.com/shivanipatel7/CapstoneProject_Coursera/blob/main/CoronaVirus%20Analysis%20with%20Forsquare%20API.ipynb

### Results: 
![alt text](https://github.com/shivanipatel7/CapstoneProject_Coursera/blob/main/results.png?raw=true)

### Conclusion: 
We can conclude that venues are not the best way to cluster corona-virus outbreak cities in the US as clustering cities based on venue categories as this resulted in overfitting. 
