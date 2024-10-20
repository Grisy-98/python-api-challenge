# python-api-challenge

### Description

This challenge was split into 2 parts and tested my skills with Python requests, APIs, and JSON transversals. 

#### Part 1
The first part was creating a Python script to visualize the weather over 500 cities of varying distaces from the equator to be able to fulfill 2 requirements. 
The first requirement was to create scatter plots to show the following relationships:
- Latitude vs. Temperature
- Latitude vs. Humidity
- Latitude vs. Cloudiness
- Latitude vs. Wind Speed

The second requirement was to compute linear regression for each relationship. Before calculating the linear regression, the data was seperated into North Hemisphere and South Hemisphere. 
Once the data was seperated, then, I created a function to create the following linear regression plots:
- Northern Hemisphere: Temperature vs. Latitude
- Southern Hemisphere: Temperature vs. Latitude
- Northern Hemisphere: Humidity vs. Latitude
- Southern Hemisphere: Humidity vs. Latitude
- Northern Hemisphere: Cloudiness vs. Latitude
- Southern Hemisphere: Cloudiness vs. Latitude
- Northern Hemisphere: Wind Speed vs. Latitude
- Southern Hemisphere: Wind Speed vs. Latitude

After each pair of plots were created, then I was tasked with describing any typr of relationship that I noticed as well as other findings that are uncovered.

#### Part 2
For this part of the challenge, I was to use my weather data skills to plan future vacations. I used Jupyter notebooks, the geoViews Python library, and the Geoapify API to create map visualizations. 
The first map displays a point for every city in the dataframe with the size of the point being determined by the humidity. 
Before creating the second map, a new dataframe is created based on given weather conditions.
Then, another dataframe is created to collect the first hotel located between within 10000 meters of the coordinates of the given city. The second map uses the information of this dataframe to plot a point for each city and each point will have a hover message with the following information being displayed:
-Longitude
-Latitude
-City
-Humidity
-Hotel Name
-Country

----

### Analysis From Part 1

#### Latitude vs. Temperature
![image](https://github.com/user-attachments/assets/baa68364-2a8f-4416-bf35-14bf8e2fe8a0)
![image](https://github.com/user-attachments/assets/949be0ae-e7cd-4f85-8b57-91f395a5c750)

The linear relationship between the latitude and maximum temperature is measured by the R-squared value, which is also called the Coefficient of Determination.
The Northen Hemisphere has a slightly strong Coefficient of Determination given that the R-squared value is 0.685. Also, the values have a negative trend, which make sense becasue as the latitude increases, meaning getting further away from the Equator, the maximum temperature gets lower.
On the other hand, the Southern Hemisphere has a moderate Coefficient of Determination given that the R-squared value is 0.563. The values here have a positive trend, which again, does make sense because as the latitude increases, meaning getting closer towards the Equator, the maximum temperature gets higher.

#### Latitude vs. Humidity


#### Latitude vs. Cloudiness


#### Latitude vs. Wind Speed
