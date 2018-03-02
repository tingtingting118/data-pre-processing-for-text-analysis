# data-pre-processing-for-text-analysis


I will apply text mining on a real data from Twitter that collected few nights ago,credit to my prof,
There are 5000 tweets with the file named "shutdown".The file has a
json format and directly collected with Twitter API. After loading the file using
json package, you should see array of 5000 tweets. 

To start with simple exploration, I only focus on several keys from the json file

Each tweet has multiple keys,

[‘text’]: The tweet’s text.
['retweeted_status']['user']['screen_name']: The username of tweet that is
retweeted (only available for retweets).


Steps for the exploration:
Step1: Load all tweets, and retweet usernames. Find out the top 5 most popular
retweet usernames

Step2: Remove duplicate tweets.Find out the number of all non-duplicated tweets (Use only unique
tweets for the next steps).

Step3: Remove URLs and mentions and rename hashtag sign to ‘hashtag_’. Vectorize
tweets using binary vectorization.Find out the top 5 hashtags used by the tweets

Step4: Map document to term matrix to 2D space and plot it using binary
vectorization. Repeat that for count vectorization and TF-IDF vectorization.
Analyze the result.

Step5: Co-occurrence analysis: Find which two hashtags appear together in a same
tweet mostly? Which two are the second most? Analyze your results.
(To measure co-occurrence between to features you can use binary
vectorization and compute the dot product between feature vectors.)  
P.S this step is unfinished as I am still trying to fix the bugs , will update soon

Step6:  Final conclusion on the exploration
