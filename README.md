# Predict how sales of weather-sensitive products are affected by snow and rain 

site: https://www.kaggle.com/c/walmart-recruiting-sales-in-stormy-weather

Walmart operates 11,450 stores in 27 countries, managing inventory across varying climates and cultures. Extreme weather events, like hurricanes, blizzards, and floods, can have a huge impact on sales at the store and product level. 

In their second Kaggle recruiting competition, Walmart challenges participants to accurately predict the sales of 111 potentially weather-sensitive products (like umbrellas, bread, and milk) around the time of major weather events at 45 of their retail locations. 

Intuitively, we may expect an uptick in the sales of umbrellas before a big thunderstorm, but it's difficult for replenishment managers to correctly predict the level of inventory needed to avoid being out-of-stock or overstock during and after that storm. Walmart relies on a variety of vendor tools to predict sales around extreme weather events, but it's an ad-hoc and time-consuming process that lacks a systematic measure of effectiveness. 

Helping Walmart better predict sales of weather-sensitive products will keep valued customers out of the rain. It could also earn you a position at one of the most data-driven retailers in the world! 

Please note: You must compete as an individual in recruiting competitions. You may only use the data provided to make your predictions.

#Evaluation

Submissions are evaluated one the Root Mean Squared Logarithmic Error (RMSLE). The RMSLE is calculated as
$$\sqrt{\frac{1}{n}\sum_{i=1}^n (\log(p_i+1)-\log(a_i+1))^2}$$
Where:

n is the number of rows in the test set
pi is your predicted units sold
ai is the actual units sold
log(x) is the natural logarithm
Submission Format

Your submission file must have a header and should be structured in the following format. The id column is a triplet representing a store_nbr, item_nbr, and date. Form the id by concatenating these (in that order) with an underscore. E.g. "2_1_2013-04-01" represents store 2, item 1, sold on 2013-04-01.


