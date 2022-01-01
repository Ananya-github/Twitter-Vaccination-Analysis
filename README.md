# Twitter-Vaccination-Analysis

To track the spread of Covid using Tweets of people tweeting their symptoms, we have mainly
focused on the new variant of covid i.e omicron and extracted tweets related to omicron and
symptoms associated with it from 26th November 2021. The reason we wanted to focus on it was
because of the less amount of work done on the new variant.
So, we tried to track those people who are vaccinated and talk about symptoms and omicrons.
Further we have to find who is vaccinated and who isn’t.
1. Track no of tweets
2. On the basis of sentiment scores and other features, we can cluster if a person will be
vaccinated or not on the basis of their tweet.


Data Extraction:
There are a few ways to collect tweets from Twitter. We can use the Twitter API but the Twitter API
limits the number of tweets we can collect, so we looked upon other methods. We can manually
scrape the tweets we want but this can be time-consuming. Another option is to use Twint. Twint
is a tool that allows us to scrape Tweets off of Twitter that fit inputted requirements. Twint allows
us to search and scrape tweets that contain certain words or phrases, tweets published by
specific accounts, tweets within a certain time frame, and much more. The code begins with
configuring the search requirements and ends with the command to run the Twint search. The
code will return the tweets that contain the term “omicron” and "symptom".

Feature Extraction:
We tried to find features that could be significant for this prediction, so we created variables like
presence of swearwords, total number of words, polarity, subjectivity, and sentiment.
Vectorisation will help us to determine the importance of a word in any tweet, and how prediction
is affected by it.

Modeling:
Our scraped data is not labelled if the person has been vaccinated or not so there is no sure
way to measure it until we do manual labelling for it. This will be a time consuming process and
may not be apt considering our current deadline. So, we decided to move forward with
unsupervised modeling i.e K-Means Clustering.
