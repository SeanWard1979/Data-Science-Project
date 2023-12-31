<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="css/app.css">
</head>
<body>

  <h1>Data Science Process: Boston-Seattle Airbnb Project <h1>

 # <h2> Installations <h2>
Python 3.8.12 and Jupyter Notebook 6.0.3

#  <h2> Project Motivations <h2>
This was a Data Science project for Udacity where I was looking to compare the Airbnb trends between 2009 and 2016 for two very large similarly populated cities on opposite sides of the United States (Boston and Seattle).  I compared the prices, number of reviews, and review scores for Boston and Seattle (by property, by neighborhood, and by entire city).  The three questions I asked were:

1. What are the most expensive neighborhoods for Airbnb for Boston/Seattle and how do they compare ?

2. Which of the most expensive Airbnb neighborhoods have the best reviewed properties between Boston and Seattle?

3. Which city has more Airbnb reviews, the best overall reviews, and the highest average prices?

#  <h2> Conclusions <h2>
-In terms of expense, Boston is a more expensive city for lodging through Airbnb.  It's a big difference both in all Airbnb properties ($167 to $127 for Seattle), and in the fact that 10 Boston neighborhoods average over $200, while only 2 Seattle neighborhoods average that high.

-In terms of the reviews of the most expensive neighborhoods, Seattle thrives with better reviews.  11 of 12 of the best reviewed expensive neighborhoods are in Seattle. 

-Also, Seattle's 94.5% rating for all reviewed Airbnb properties far exceeeds Boston's 91.9% average.  This is a significant difference when it comes to reviews.

-Seattle has far more total reviews than Boston (84,829 to Boston's 68,208).  My theory is that because Airbnb was started on the west coast (San Francisco in 2008), it is more established in Seattle than it is in Boston.  

-Also of interest: They are very similar in population (726,000 in Seattle, 672,800 in Boston as per https://www.bestplaces.net/compare-cities/seattle_wa/boston_ma/people) but Seattle takes up far more space (almost twice as much with 84 square miles as compared to Boston's 48.3 square miles as per https://www.quora.com/Is-Seattle-bigger-than-Boston-Is-it-how-much-bigger).  This also explains why Seattle has far more neighborhoods than Boston.

#  <h2> File Descriptions <h2>
-Original Data Sets-

https://github.com/SeanWard1979/Data-Science-Project/blob/main/Seattle_listings.csv

[Seattle_listings.csv] : The dataset featuring all of the Seattle Airbnb listings from 2009-2016 

https://github.com/SeanWard1979/Data-Science-Project/blob/main/listings.csv

[listings.csv] : The dataset featuring all of the Seattle Airbnb listings from 2009-2016

-Cleaned Data Set-

https://github.com/SeanWard1979/Data-Science-Project/blob/main/df_merged.csv

[df_merged.csv] : The Boston and Seattle datasets cleaned and merged with many columns dropped (the originals had 92 columns, this one has 9 columns).

-Final Notebook and References-

(https://github.com/SeanWard1979/Data-Science-Project/blob/main/Data_Science_Process_Boston-Seattle_Airbnb_Final.ipynb)
[Data_Science_Process_Boston-Seattle_Airbnb_Final.ipynb] : Featurings all of the data cleaning, wrangling, exploration and visualizations of the project with the questions and conclusions as well.

(https://github.com/SeanWard1979/Data-Science-Project/blob/main/References.ipynb)
[References.ipynb] : All of the websites that I explored to help me code.

#  <h2>The Project's Journey <h2>
I started off with two very large datasets for Seattle and for Boston (both 92 columns) and explored through what each column looked like while looking at the source of the data (kaggle.com).  I was able to choose the 14 initial columns that I wanted to explore for the project while I was importing the .csv files from kaggle.com.  Some columns I didn't use (but what could still work for further exploration) were the Airbnb host's name, street, bathrooms, bedrooms, amenities, along with latitude and longitude (for geospatial visualizations aka maps).

After I came up with the three questions, I dropped the columns I wasn't going to use.  I did some data cleaning to drop all of the Nan values and to make sure all cities said either "Boston" or "Seattle."  After I cleaned each one up, I merged them into one dataset called "df_merged." 

Question 1: What are the most expensive neighborhoods for Boston/Seattle and how do they compare?
I decided to start grouping the data by "neighborhood" to look at the average values especially for price.  I decided that there were way too many neighborhoods to have a visualization that has all of them on it...so I narrowed it down to the 15 most expensive neighborhoods in Boston and the same for Seattle.  I created a dataset (neigh_merged) for these 30 neighborhoods, sorted them in descending order, then created a horizontal bar chart.  The bar chart clearly showed that Boston had 12 of the 14 most expensive neighborhoods.

Question 2: Which of the most expensive Airbnb neighborhoods have the best reviewed properties?
I reused the neigh_merged dataset to compare the 30 most expensive Airbnb neighborhoods by review score averages.  In the bar chart I created, it showed that Seattle's expensive neighborhoods were rated higher (11 of the first 12 highest rated were Seattle).  With the previous horizontal bar chart and this bar chart I used the color "blue" for Seattle and the color "red" for Boston (a nod to the Mariners and Red Sox baseball teams).  

Question 3: Which city has more Airbnb reviews, the best overall reviews, and the highest average prices?
In continuing to compare reviews and prices, I decided to look at overall numbers for both Boston and Seattle.  I dropped all the entries that had "0" for number of reviews and called that dataset "reviews."  I made sure they all had the city name for each line, and created comparisons between Boston and Seattle for averages and for sums.  The averages were for price, number of reviews and ratings.  The sums were mostly for number of ratings. 

I created a pie chart that counted the total number of reviews for Boston and Seattle (Seattle= 55.4% and Boston= 44.6%).  I had another bar chart showing the number of reviews (Seattle= 84,829, Boston= 68,208).  I also created a stacked bar chart showing average price, number of reviews, and review score ratings between Boston and Seattle. It all verified that Boston has the higher average price by far ($167 to Seattle's $127) and that Seattle had slightly more reviews per property (Seattle= 26.8, Boston= 24.6).  Seattle also had higher average review scores as well (94.5% to 91.9% for Boston).  


#  <h2> Licensing, Authors, Acknowledgements, etc. <h2>
This data was taken from: 
https://www.kaggle.com/datasets/airbnb/seattle/data  for Seattle.
https://www.kaggle.com/datasets/airbnb/boston/data for Boston

Author: Sean Ward

</body>
</html>
