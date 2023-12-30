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
Seattle_listings.csv : The dataset featuring all of the Seattle Airbnb listings from 2009-2016 
listings.csv : The dataset featuring all of the Seattle Airbnb listings from 2009-2016

-Cleaned Data Set-
df_merged.csv : The Boston and Seattle datasets cleaned and merged with many columns dropped (the originals had 92 columns, this one has 9 columns).

-Final Notebook and References-
Data_Science_Process_Boston-Seattle_Airbnb_Final.ipynb : Featurings all of the data cleaning, wrangling, exploration and visualizations of the project with the questions and conclusions as well.
References.ipynb : All of the websites that I explored to help me code.

#  <h2> How to Interact with your project <h2>
Feel free to download my Final Notebook, explore more with the code and then post your own version of the notebook on here.


#  <h2> Licensing, Authors, Acknowledgements, etc. <h2>
This data was taken from: 
https://www.kaggle.com/datasets/airbnb/seattle/data  for Seattle.
https://www.kaggle.com/datasets/airbnb/boston/data for Boston

Author: Sean Ward

</body>
</html>
