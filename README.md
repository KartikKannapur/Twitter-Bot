Twitter-Bot
===========

Twitter bots are computer programs that watch every public tweet on Twitter. When a bot finds a tweet with a certain keyword or addressed to a Twitter account, it either sends a pre-written response, re-tweets or it follows the Twitter account.
In my case I have created a Bot @CodeTerminal

Resources 
=========
The Websites / Services we will use:
1. Feedburner - http://feedburner.google.com.  If we use Yahoo Pipes directly with a Twitter search, it will access the Twitter servers too frequently which will result in errors and timeouts.  Feedburner only updates a feed either every 30 minutes or when notified with a ping. This means that we can be kinder to Twitter’s servers and will have more consistent data.  

2. Yahoo Pipes - http://pipes.yahoo.com.   We use Yahoo Pipes to clean up the results we get back from Twitter.

3. Twitterfeed - http://twitterfeed.com.  We use Twitterfeed to actually post/tweet the data from Yahoo Pipes feed.

Setup 
=========
1. Source:
We want to auto-retweet any tweet that mentiones the account - @CodeTerminal. The Twitter Search API is part of Twitter's v1.1 REST API. Search for the account @CodeTerminal in the Twitter Search Bar, the URL loaded will be something like this - https://twitter.com/search?q=%40CodeTerminal.
   
Replace "https://twitter.com/search" with "https://api.twitter.com/1.1/search/tweets.json" and you will get -           https://api.twitter.com/1.1/search/tweets.json?q=%40CodeTerminal

To use the RSS Feed option : 
Go to http://www.queryfeed.net/ and Search Twitter for @CodeTerminal. 
Copy the URL, should look like this - http://www.queryfeed.net/twitter?q=%40CodeTerminal&geocode= and paste it at http://feedburner.google.com/ and Burn the Feed.
Feed Title : Twitter feed for '@CodeTerminal' query
Feed Address : http://feeds.feedburner.com/TwitterFeedForcodeterminalQuery
   

2. Twitter Account:
   You can either use an existing Twitter account or create a new one for your Bot.

3. Feedburner:

