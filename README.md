# Inland-Ontario-Lakes-Trends-Capstone
 
 Problem
 The problem being addressed in this capstone is an exploration into historical trends and patterns between dissolved oxygen and other factors including temperature, depth, season, and lakes. This data are measurements from 9 lakes in Ontario between 1976-2021. 
 We will be addressing below research questions: 
  1. What are long term and seasonal trends within the water temperature and dissolved oxygen between 1976-2021 across 9 Ontario lakes? 
  2. How do the temperatures vary across lakes and at different depths? 
  3. What is the relationship between temperature and dissolved oxygen, and how are these varying across lake, depth, and season? 
 
Dataset source
 The dataset source is from Government of Ontario — Inland Lakes and Streams: Physical Conditions. Raw dataset includes 104,319 rows and 10 columns. 3 columns were added (Year, Month, and Season) which were derived from the date variable. Variables include: Lake, District, Township, Latitude, Longitude, Date, Year, Month, Season, Depth, Temperature, and Dissolved oxygen.

Methodology and Approach
1. I inspected the data and identify and understand the variables being used. I identified the missing variables and perform descriptive statistics on the variables to understand the spread.
2. I cleaned and prepared the data by adding 3 columns as discussed above. For the exploratory data analysis, I created several graphs and plots, including: bar, histogram, box and whisker, scatter, and line graphs. I also performed a correlation matrix.
3. I created training and testing data with an 80/20% ratio based on the number of datapoints in each year chronologically. I created a baseline and linear regression model since our target variable, dissolved oxygen, is a continuous numerical amount.
4. I evaluated and interpreted metrics conducted for both models for comparison. Metrics included MAE, RMSE, and R^2. Limitations of the model and data were also stated in this section.

Model Development
For the rows missing observations from either dissolved oxygen or temperature were removed when performing the baseline and linear regression model.
In the baseline model, I used the mean of the dissolved oxygen and for the linear regression, the analysis included other environmental variables(temperature, depth, year, lake, and season).

Dependencies
Project utilized Python in Google Collab. Libraries used include: Pandas, Numpy, Matplotlib, and Scikit-learn

Limitations
There are a few limitations in the data including missing observations and uneven distribution of data points between years. For testing and training purposes, I analyzed the data chronologically and split the earlier years from 1976-2011 as training and 2012-2021 as testing.
 
