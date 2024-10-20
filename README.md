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

Note: When creating the function, I had help from the Xpert Learning Assistant. I modified the given code to not use the seaborn library as well as added annotations to the graph so the linear equation can be displayed. 

After each pair of plots were created, then I was tasked with describing any typr of relationship that I noticed as well as other findings that are uncovered.

#### Part 2
For this part of the challenge, I was to use my weather data skills to plan future vacations. I used Jupyter notebooks, the geoViews Python library, and the Geoapify API to create map visualizations. 
The first map displays a point for every city in the city_data_df DataFrame with the size of the point being determined by the humidity.
![image](https://github.com/user-attachments/assets/a213f288-8af7-4823-baf4-2d9f04c4d9ae)

Before creating the second map, a new dataframe still called city_data_df DataFrame is created based on my ideal weather conditions, which are:
- A max temperature between 20 and 30 degrees
- Wind speeds less than 10.5 m/s
- Zero cloudiness
- Dropping any rows with null values

Then, another DataFrame, called hotel_df is created to collect the first hotel located between within 10,000 meters of the coordinates of the given city. The second map uses the information of hotel_df to plot a point for each city and each point will have a hover message with the following information being displayed:
-Longitude
-Latitude
-City
-Humidity
-Hotel Name
-Country
![image](https://github.com/user-attachments/assets/47396705-0ea5-426b-89c8-588d813c7c54)

----

### Analysis From Part 1

#### Latitude vs. Temperature
![image](https://github.com/user-attachments/assets/baa68364-2a8f-4416-bf35-14bf8e2fe8a0)
![image](https://github.com/user-attachments/assets/949be0ae-e7cd-4f85-8b57-91f395a5c750)

The linear relationship between the latitude and maximum temperature is measured by the R-squared value, which is also called the Coefficient of Determination.
The Northen Hemisphere has a slightly strong Coefficient of Determination given that the R-squared value is 0.685. Also, the values have a negative trend, which make sense becasue as the latitude increases, meaning getting further away from the Equator, the maximum temperature gets lower.
On the other hand, the Southern Hemisphere has a moderate Coefficient of Determination given that the R-squared value is 0.563. The values here have a positive trend, which again, does make sense because as the latitude increases, meaning getting closer towards the Equator, the maximum temperature gets higher.

#### Latitude vs. Humidity
![image](https://github.com/user-attachments/assets/22a8848f-c3c0-43cc-b660-499c43865b9d)
![image](https://github.com/user-attachments/assets/db76a1db-e072-448d-aee9-bf3814843ad8)

The linear relationship between the latitude and the humidity is really weak, which means that the humidity is not dependent on the latitude. Even without finding the R-sqaure value, the scatter plot shows that all the points are scattered around, and there is no trend.

#### Latitude vs. Cloudiness
![image](https://github.com/user-attachments/assets/c2819734-91e1-4892-8266-4a97a9cdec9f)
![image](https://github.com/user-attachments/assets/fb8124f8-5937-42ed-8881-dc0c30c1fc24)

Similar to latitude vs. humidity, the linear relationship between the latitude and the cloudiness is really weak, which means that cloudiness is not dependent on the latitude. Even without finding the R-sqaure value, the scatter plot shows that all the points are scattered around, and there is no trend.

#### Latitude vs. Wind Speed
![image](https://github.com/user-attachments/assets/021f32c1-5384-4bb1-86e6-06c8700c3e85)
![image](https://github.com/user-attachments/assets/7f13aa3c-419c-4f3e-ba95-cf3842a3896f)

The linear relationship between the latitude and the wind speed is really weak, which means that the wind speed is not dependent on the latitude. Even without finding the R-sqaure value, the scatterplot shows that all the points are scattered around, and there is no trend.
