# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
1. Accessing data using APIs
2. Cleaning and transforming data using Python
3. Loading data into a database using Python
4. Performing EDA, including using both statistics and visualizations
5. Identifying trends and patterns in data using statistical models
6. Interpreting the results of the statistical models


## Process
1. Connecting to CityBikes API to retrieve Quebec, Canada bike stations information
   1) Explore all citybikes api information, chose Quebec, Canada API
   2) From Quebec, Canada API, retrieve data of each bike station's latitude, longitude and number of bikes
   3) Parse the information into a Pandas dataframe, and save as a .csv file

2. Connecting to Foursquare and Yelp APIs to get restaurants information
   1) From Foursqure and Yelp API, retrieve restaurants information for each of the bike stations
   2) Parse Restaurant POIs into a Pandas dataframe, and save as a .csv file

3. Joining Data
   1) Join Quebec, Canada bike stations dataframe with restaurants dataframe 
   2) Explore the relationship between the data
   3) Store all dataframes into SQLite database, explore the data before and after join

4. Building a Model
   1) Building a multivariate linear regression model
   2) Repeating to remove p-vaule > 0.05 variable at one time
   3) Training the model to get the best fit


## Results
Yelp API provides more detail information, such as review count, rating, 
the restaurants whether is closed etc. Besides, Yelp API can retrieve more
restaurant records

From the modelling results, p-value < 0.05 for all varialbes. 
The coefficent values also shows that restaurant's longitude 
has strong positive impact on the number of bikes, 
its longitude has negative impact on the number of bikes. 
But Adj. R-squared is 0.098 , it shows that 
this multivariate model only explains 9.8% of the variations in the data. 


## Challenges 
TThe challenges I faced in the project are connecting API to access data, 
and performing EDA, and building the model


## Future Goals
The multivariate model performance is not good, This is because data 
doesn’t meet the model requirements. If I had more time, I will perform 
EDA in depth, and use scale method to make sure data meets the model requirements 


