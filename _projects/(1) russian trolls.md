---
name: Classifying Tweets from Russian Trolls
tools: [Python, Data Science, NLP, Data Viz, Twitter]
image: https://raw.githubusercontent.com/yontartu/yontartu.github.io/master/images/russian_trolls/tweets_thumbnail.png
description: I built a machine learning model that predicts whether a tweet is from a "Right Troll" account controlled by the Russian government. 
---


# Classifying Tweets from Russian Trolls

<br>
This project involved building a machine learning model to detect tweets from Twitter accounts controlled by the Russian government. During the 2016 U.S. presidential campaign, the Russian government promulgated a disinformation campaign on Twitter through its Internet Research Agency. Today Twitter continues to grapple with disinformation on its social network. My model seeks to use information embedded within the text of a tweet to predict whether a tweet is likely to be associated with a Russian troll account. I made use of a [dataset of labeled tweets](https://github.com/fivethirtyeight/russian-troll-tweets) originating from confirmed Russian government accounts, as well as a dataset I constructed of tweets from verified Twitter users. 

The tool below lets you explore some of the tweet-level predictions from my model. Each dot represents a tweet, colored by whether it originated from a Russian troll account (red) or a verified user (turquoise). Hovering over a dot will show you more information about the tweet, including the predicted probability of the tweet coming from a Russian troll as well as the original text of the tweet. 

To make predictions on new tweets, check out the accompanying [web app](https://russian-troll-detector.herokuapp.com/).

<br>
<iframe src="/images/russian_trolls/explore_tweet_predictions.html"
    sandbox="allow-same-origin allow-scripts"
    width="1000"
    height="600"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>  
Source code can be found on [my GitHub](https://github.com/yontartu/bot-vs-human).



