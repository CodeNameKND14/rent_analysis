Graphing Rent: What variables are National rent prices dependent on?

Group: Null_Value

Members: 
Adam Dunbar, Sergio Fidanli, Kendall Jackson, Max O’neill, Finn Wurtz

---------------------------------------------------------------------------------------------------------------------

Question: How do population dynamics affect Rent Pricing in America’s most populated 250+ cities? 
As one might imagine, our analysis shows that the larger the city the more competition there is for housing on the rental market. This leads directly to higher rental prices than in cities with lower populations and lower housing demand. As shown in the graph below, there is a positive relationship between population and the rental prices of housing in cities. 

However, if you consider the two most populated cities in the US (New York and Los Angeles) to be data outliers (and remove their data points), then the positive relationship disappears and there is a neutral relationship between population and rent pricing (a flat linear regression line with no slope). That being said, it is important to include these major cities into our analysis to really understand the urban dynamics at play here (at least in terms of population).

Perhaps the most significant relationship observed between our various variables and rent prices was with that of Population Density. Cities with limited suitable building area due to being located on islands (New York City) or peninsulas (San Francisco) are often more densely populated. As a result, the demand and intense competition for existing housing leads to higher than average rental prices (and in the case of San Francisco the highest in the US).


Question: Does Weather Play a Factor on Rental Price?
For this question, we decided to use data from the NOAA (National Centers for Environmental Information) as they provide historical data for both average temperature and precipitation. We decided that a 5 year average from Jul 2014 to June 2019 would be a good time period as it would show recent trends in weather patterns. 

We suspected warmer climates would be more desirable, yielding increased rent cost, but looking at the data, it doesn’t seem to play much of a factor. 
A stronger relationship occurs when we plot the average 5 year precipitation levels (in inches) vs. the average median rent. We suspected that areas receiving more rain are less desirable and we see some evidence that is in fact the case. 
Overall, we conclude that weather doesn’t play much of a factor at all. It seems that people will tolerate colder weather (or more rain) for higher paying jobs. For instance, Seattle is a city known for its rainy days, but also very high cost of living.


Question: Do Economic Factors Such as Unemployment Rate and Wage Growth Play a Factor on Rental Price?
For this question, we decided to use data from the Bureau of Labor Statistics (BLS). Annual wage growth for 2018 was available at the county level and annual unemployment rate for 2018 was available at the city level. 
As expected, we see a positive relationship between wage growth and rental price, however the relationship is not as strong as we thought it would be. Perhaps wage growth for the cities with higher rent are stagnant. Maybe there is a lag between wage growth and rent price. It would be useful to plot high wage growth for 2016-2018 and then look at the change in rent from 2016-2018.

Same thing for unemployment rate; slightly positive linear relationship but not as strong as we hoped. Again, for further analysis we may want to look further back and calculate the change and see how it compares to rental growth over a multi-year period. Perhaps unemployment rate can be low but most jobs aren’t high paying.



Question: Does location of Colleges and Universities play a factor on rental price?
For this question, we decided to use data from Google Maps Place Search API as it provides data for specified locations. We suspected that the more universities and colleges around a certain location, the higher the rent prices for that location would be. Comparing the number of Universities located near each city from a 50,000-mile radius seems to show a weak positive linear correlation. There is something to say about Universities and Colleges and their existence to where you live, however, we have concluded that this correlation was not strong enough to say with certainty that the amount of universities existing where you live impacts rent prices.



Question: Does location of Sport Stadiums play a factor on rental price?
For this question, we used data from Google Maps Place Search API as it provides data for specified locations. We suspected that the more Sport Stadiums that were around a certain location, the higher the rent prices for that location would be. Comparing the number of Sport Stadiums located near each city from a 50,000-mile radius seems to show a very weak positive linear correlation. Though this shows a positive regression line the plot seems to be more scattered and nonlinear. We have concluded that, based on our data, there is no correlation between sports stadiums and high rent prices. 



Question: Can We Build a Model That We Can Use to Predict Rent Price? Can We Use the Results to Quantify How Overpriced West Coast Cities Are?
We had the idea to use temperature data, economic data, and other datasets to build a linear regression model that could explain what factors drive up the cost of rent (also demand) for a city. By training the data on American cities where the median rent of a 1 Bedroom apartment is < $2,000, we could fit a model that applies to the vast majority of cities. If the model predicts well, we could run it on cities with large rents (>= $2,000/mo) in California, New York, Washington, etc. to quantify just how overpriced they are.

Unfortunately, the factors we were able to obtain weren’t very predictive. Our best version of the regression model only contained enough data for 74 cities and when using a 80%/20% train/test it’s just not enough data to be able to trust the model’s results. The RMSE is $210 which is 18% of the average 2019 rent price.

In summary we are definitely missing some key data that would help build a better model. Maybe the % of tech workers per capita, or % of people with bachelors or advanced degrees per capita. Some factor that brings in the jobs that generally pay more.



Question: Can Unemployment due to Education, affect rent?

By using BLS once again for our data source, this particular question is to find out if education was a major impact on unemployment which could possible lead to rent decreasing and/or increasing. BLS has conducted a survey to show the percentage of unemployment for different Levels of Education that Americans were catergorized in. Throughout a ten year span, right after the 08’ crash to be specific, there are 4 demographics; No High School Diploma, High School Diploma, Associates Degree or Cert. and Bachelor’s or Higher. 

The First 3 were affected the most considering the level of Education that they had and were not able to get a job right after the crash but for those that had a bachelor’s degree or higher were relatively secure in the workforce. Now these four demographics were working in 5 specific industries listed as; Business Services, Medical, Manufactoring, Construction and Technology.   

Though there is not enough data to really show that education had an impact on rent or not however, the increase of jobs and the requirements of education to get those jobs is a potential factor down the road.
