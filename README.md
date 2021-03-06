#  **Weather Analysis Using Python and GoogleMaps API**

**Weather Analysis:** Created a dataset of 500+ random cities using OpenWeatherMap API to analyze weather patterns as a function of equatorial distance.  

**Vacation Analysis:** Filtered cities based on weather variables and used GoogleMaps API to find and map my ideal vacation spots. 

Data Analysis, linear regression and visualizations conducted using Python, Pandas, Citipy, Plotly, Gmaps, and Matplotlib.

![Weather Analysis](https://github.com/mocchicone/Weather-Analysis-Python-GoogleMaps/blob/master/Images/heatmap_2.png)

## **Weather Analysis**

### **Step 1:**
Used Python, Numpy, and Citipy to generate a list of 500+ cities based on random latitude and longitude coordinates.  
  
### **Step 2:**
Made an API call (get request) on 7/12/2020 to OpenWeatherMap to grab weather data for each of the cities which was then converted into a pandas dataframe.
  
### **Step 3:**
Used Matplotlib to conduct simple linear regression analysis on the input variable (latitude) and our four dependent variables (max temperature, humidity, cloudiness, wind speed) accross two groups (northern hemisphere and southern hemisphere).  

![Scatter1](https://github.com/mocchicone/Weather-Analysis-Python-GoogleMaps/blob/master/Images/scatter_lat_temp.png)![Regression1](https://github.com/mocchicone/Weather-Analysis-Python-GoogleMaps/blob/master/Images/regnh_lat_temp.png)
  
### Weather Observations:

1. There is a significant correlation between latitude and Max Temp as run on July 12, 2020, so that the further away from the equator, the warmer the max temperature.  The effect size is stronger in the southern hemisphere (r2 = .65), than in the northern (R2 = .44)

2. Latitude is not a significant preditor of Humidity, Cloudiness, or Wind Speed

3. As the weather data was pull in July, additional analysis could be conducted by using the same list of cities and calling the API during the winter to see if time of year impacts the strength of the relationships between the variables.

## **Ideal Vacation Location**

Based on my ideal weather conditions for a pleasant vacation, I created a heatmap using Gmap, filtered the data down to five cities, and used the Google Maps API to locate the nearest lodging and added them to the heatmap as a marker layer.  

### **Step 4:**
Used Gmaps, Python, and Pandas to create a heatmap of the 500+ cities based on humidity.

![Heatmap](https://github.com/mocchicone/Weather-Analysis-Python-GoogleMaps/blob/master/Images/heatmap_1.png)

### **Step 5:**
Filtered the cities dataset by ideal conditions for wind speed, humidity, cloudiness, and max daily temperature resulting in a list of five cities.
  
### **Step 6:**
Used a GoogleAPI get request to locate one lodging within each of the five cities. Appended the lodging as a marker onto the heatmap.

![Heatmap Markers](https://github.com/mocchicone/Weather-Analysis-Python-GoogleMaps/blob/master/Images/heatmap_2.png)
  
**Contact:**   
Michael Occhicone: mpocchicone@gmail.com 





