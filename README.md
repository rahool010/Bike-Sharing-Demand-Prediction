
<h1 align="center">  Bike Sharing Demand Prediction
 </h1>

<h3 align="center"> AlmaBetter Verified Project - <a href="https://www.almabetter.com/"> AlmaBetter School </a> </h5>


![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Project Summary
Bike sharing system is an innovative transportation strategy that provides individuals with bikes for their common use on a short-term basis for a price or for free. Over the last few decades, there has been a significant increase in the popularity of bike-sharing systems all over the world. This is because it is an environmentally sustainable, convenient and economical way of improving urban mobility. In addition to this, this system also helps to promote healthier habits among its users and reduce fuel consumption.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Problem Statement
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Dataset Information
Dataset used in this project is the Seoul Bike Share program data.This dataset contains information about the total count of rented bikes at each hour, as well as the date of observation and meteorological information (Humidity, Snowfall, Rainfall, Temperature Season, and so on) for that hour. The observations in the dataset were recorded during a span of 365 days, from December 2017 to November 2018.

The Seoul Bike Dataset contains the following information:

* **Date** - The date of each observation in the format 'year-month-day'
* **Hour** - Hour of the day
* **Temperature** - Temperature recorded in the city in Celsius (°C).
* **Humidity** - Relative humidity in %
* **Wind speed** - Speed of the wind in m/s
* **Visibility** - measure of distance at which object or light can be clearly discerned in units of 10m
* **Dew point temperature** - Temperature recorded in the beginning of the day in Celsius(°C).
* **Solar radiation** - Intensity of sunlight in MJ/m^2
* **Rainfall** - Amount of rainfall received in mm
* **Snowfall** - Amount of snowfall received in cm
* **Seasons** - Season of the year (Winter, Spring, Summer, Autumn)
* **Holiday** - Whether the day is a Holiday or not (Holiday/No holiday)
* **Functional Day** -Whether the rental service is available (Yes-Functional hours) or not (No-Non functional hours)

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Tools and Technologies used
The programming language used in this project is Python. The following libraries were used for data analysis and data visualization and to build a recommender system.

* **Pandas** : For loading the dataset and performing data wrangling.
* **Matplotlib**: For data visualization.
* **Seaborn**: For data visualization.
* **NumPy**: For some math operations in predictions.
* **Statsmodels**: For statistical computations.
* **Sklearn**: For the purpose of analysis, prediction and evaluation.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Steps Performed
* **Data Preprocessing** : Checked for outliers, incorrect values, missing values, duplicate, performed data type correction and string formatting.
* **Merging of datasets** : In this project, recommender systems were built utilizing only explicit ratings . So finally,a new dataframe by merging the books dataset ,explicit ratings dataset and users dataset.
* **Feature Extraction** : Created new columns such as age_group by binning the 'Age' column and extracted the country name from the 'Location' column .
* **Exploratory Data Analysis** : Performed Univariate, Bivariate, and Multivariate analysis with various graphs and plots to better understand the distribution of features and their relationships.
* **Implementation of various Recommender System approaches.**

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## Conclusion
We found that Linear Regression performed poorly as expected. Decision Tree and Random Forest showed overfitting. The best performance was given by the XGBoost model.

1. The Mean Absolute Error for training and test set was 134 and 152 respectively which was lesser compared to previous models.
2. The Root Mean Squared Error for training and test set was 216 and 244 respectively which was lesser compared to previous models.
3. The R2_score and adjusted r2_score was 0.88 and 0.84 which was higher compared to all the other models. 
 
 
Also implemented shap technique to understand the working of our XGBoost model:
* Temperature was the most important feature. Demand for bikes was higher when temperature was high.
* Hour of the day was the second most important feature. Demand was high during evening hours.
* Demand was less in winter season as compared to other seasons.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)