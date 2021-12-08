# CSCI2000U_FinalProject

### Pfizer Vaccine Tweets

###### About  me:
Name : Prachi Sharma
Github username : 

#### Introduction:
Covid 19 has affected millions around the world. Therefore, it is no surprise that the developement of vaccines has encouraged great amount of discussion around the same. People are keen to express their opinions(positive or negative) on social media. However, such opinions may influence thousands of other users too. The above dataset contains tweets about Pfizer & BioNTech vaccine. The goal of choosing this dataset is to examine how an common twitter user feels about the vaccine along with determining interaction on different accounts(with regards to their followers,friends,location etc). The dataset can also be used to determine if a more popular twitter opinion might influence other users. 

###### Description of Data
The dataset is a csv file which contains tweets about Pfizer & BioNTech vaccine over two years(2020 and 2021). The data was collected using tweepy Python package to access Twitter API. The source of the datset was Kaggle. 
Source: https://www.kaggle.com/gpreda/pfizer-vaccine-tweets?select=vaccination_tweets.csv

#### Conclusion
The dataset chosen by us showed great potential for data science applications. The said dataset contained tweets made by twiiter users from various locations about pfizer vaccine. To make dealing with the given data easier, we cleaned different columns such as date and text. For cleaning the date column, to_datetime function was used to convert the objects in the date column to datetime objects. Further, we learnt to extract only month and year from the date in two separate columns. In datasets containg tweets, preprocessing of tweets is necessary to analyse our data better. We learnt to remove all special characters such as hashtags,mentions,emojis,punctuations and numeric digits from the tweets.

A pivot table containg the number of tweets made per month and year was also constructed. The pivot table gave us an idea about the timeline during which tweets about the pfizer vaccine were being tweeted the most. Further, by finding the number of unique usernames, we were also able to deduce that some users tweeted more than once on the said topic. The top 10 users who tweeted the maximum number of tweets were shown above with the help of the bar chart. Similarly, we were also able to find out the top 10 locations from where the maximum number of tweets were made. The bar chart displaying the same is displayed above

We also learnt to construct a wordcloud. Wordcloud was used to display the most frequent words used in a tweet. This can be helpful in getting to know the general consensus amongst the users.

Lastly, we also used Vader sentiment analysis to analyse the general sentiment of the tweet. We learnt to classify tweets as being positive,negative or neutral based on the compound score

#### Limitations and possibilities for refinement:
For further enhancing our analyis, we could try to experient with different sentiment analysis methods. It would be interesting to test out how different methods compare to each other in terms of accuracy.

Furthermore, we could also try to measure the influence of positive/negative tweets made in a country to the vaccination drive taking place over there. This would be done with by accessing different data about the vaccination drives. Then, we would be able to conclude if positive/negative tweets hold any significant influence.

The bar chart displaying the top 10 locations from where the maximum number of tweets were made is not necessarily accurate. The value_counts() function counts a particular country and a city inside that country as two separate locations. For instance, India and Chennai, India are counted as two separate locations. We could try to define a function which would classify the a city inside a country and the said country as two separate locations.

