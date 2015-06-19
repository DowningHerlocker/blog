measuring-emotions-on-reddit
===

<<<<<<< HEAD
In order to analyze human emotion in social networks, I used sentiment analysis on comments from the 50 top subreddits. In this post, you'll see how I parsed through reddit's somewhat messy API, and found the sum sentiment scores for the top 50 subreddits. 

Reddit, is more than just a place to get updated on worldnews, look at cute pictures of puppies, and hear about the latest edition of world of warcraft. Reddit has become a community where millions of people gather every day to view and post their thoughts, opinions, and views on thousands of different topics. Reddit has a straightforward JSON API; access a JSON representation of any page by appending '.json' to the URL. Here is a comment taken from the subreddit [aww](http://www.reddit.com/r/aww/comments/3a1cba/this_is_ollie_hes_ready_for_business). 



I parsed the API, taking out the relevant information needed for my analysis. Here is a sample of my cleaned-up json:



- - -

With my new easy to navigate json, I ran a sentiment analysis test on all of the comments of each post on each subreddit. Sentiment, created by [@thisandagain](https://github.com/thisandagain, is a Node.js modulue that uses a preset worldlist, where each block of test is scored based on the negative or positive value of each word. Below is an example of how the sentiment analysis works:

```
"You're dad is adorable and I want to adopt him." -Score: 5
"It is incredible how many idiots are around us. Reddit is an idiot magnet" -Score: -3
```
Sometimes, the sentiment scores can be off, due to sentiment's failure to understand context, as seen below:

```
"Holy fuck. That's like weaponized cuteness right there." Score: -2
```

However, by examining thousands of comments, the sum score pretty much averages out. 

- - -

Aside from the easy to access API, I chose to anaylyze reddit because it covers such a broad range of topics, and is utilized by such a wide range of people. I performed the analysis on the top 50 subreddits. 

This graph shows the sum sentiment scores of the top 50 subreddits from negative to positive. 



As you can see, the subreddit "IAmA" has the highest sum sentiment scores. With the "I Am A" subreddit, users post what they do in life, and people can comment, ask questions, ect. The subreddit with the most negative sum sentiment score was "AskReddit", where users can ask reddit anything. 

- - -
After analyzing the top 50 subreddits, I looked into contrasting subreddits.

###Highlight comparisons###

                                                Cats vs Dogs


                                        Replublicans vs Democrats


- - -

Finally, I analyzed the top 25 U.S. cities. The top 25 cities ranked according to population and rank respectively include: 

```
1.New York City         6. Philadelphia         11. Austin              16. Fortworth           21. Denver 
2.Los Angeles           7. Phoenix              12. Jacksonville        17. Charlotte           22. Washington DC     
3.Chicago               8. San Antonio          13. San Francisco       18. Detroit             23. Memphis
4.Houston               9. Dallas               14. Indianapolis        19. El Paso             24. Boston
5.Philadelphia          10. San Jose            15. Columbus            20. Seattle             25. Nashville
```

Here you can see the different sum sentiment scores of each U.S. city. 




Whether you want to analyze how people feel about your favorite sports teams, the country you're visiting this summer, or the candidates for the presidential election, using sentiment anaylsis can quickly determine the human emotions on thousands of different topics. 

- - -
=======
In order to analyze human emotion in social networks, I used sentiment analysis on hundreds of comments on reddit.com. In this post, you'll see how I parsed through reddit's somewhat messy API, and found the sum sentiment scores for the top 50 subreddits. 

Reddit, is more than just a place to get updated on worldnews, look at cute pictures of puppies, and hear about the latest edition of world of warcraft. Reddit has become a community where millions of people gather every day to view and post their thoughts, opinions, and views on thousands of different topics. Reddit is great because it's public API allows access to lots of useful data just by adding ".json" to the end of the post's url. However, as you can see below, the API is somewhat hard to navigate. 

[picture of json]

I parsed the API, taking out the relevant information needed for my analysis. Here is a sample of my cleaned-up json:

[picture of my pretty json]

With my new easy to navigate json, I ran a sentiment analysis test on all of the comments of each post on each subreddit. Sentiment is a Node.js modulue that uses a preset worldlist, where each block of test is scored based on the negative or positive value of each word. Below is an example of how the sentiment analysis works:

['I love puppies so much. They're just the best! -Score: 12]
[I can't believe I am graduating college today. I am going to miss my friends. -Score: 2]

Sometimes, the sentiment scores can be off, due to sentiment's failure to understand context, as seen below:

[This puppy is so damn cute. I might squeeze it to death. -Score: -4]

However, by examining thousands of comments, the sum score pretty much averages out. 

Aside from the easy to access API, I chose to anaylyze reddit because it covers such a broad range of topics, and is utilized by such a wide range of people. I performed the analysis on the top 50 subreddits. Below, you can see that the top 15 subreddits alone cover material of all types. 

[picture of top 15 subreddits]

This graph shows the sum sentiment scores of the top 50 subreddits from negative to positive. 

[picture of all 50 subreddit scores]

As you can see, the subreddit "IAmA" has the highest sum sentiment scores. With the "IAmA" subreddit, users post what they do in life, and people can comment, ask questions, ect. Let's look at a few posts in this subreddit to see what sentiment analysis found. 

[Subreddit: I Am A
Post: "We're the Google Flights team, makers of flight search related stuff. Ask us anything!"]

This post in particular had 329 total comments, which I easily found from parsing the API. Of the 329 comments, there were some negative comments, such as:
 	
 	["Why did you eliminate the list view of flights? The graphic map might be neat to look at but it is a time waster for business travelers. You lost my business." Score: -3]

 and many positive comments, such as:

 	["First. I'd like to say thank you for making an amazing tool which works so well and fluidly. I often go on it for fun to see where I could go with 'x' amount of money. \n\nI was wondering if there will be any chance of being able to compare flights by area or region. For example, I live in NW England and I have about 3 nearby international airports and it'd be great to be able to say all airports in England or list several airports. \n\nAnd also, what would need to be done for Google to analyse patterns and try to predict when the cheapest flight will be available for booking for going on a certain date? \n\nKeep up the amazing work you do! Your amazing tool meant I could go on holiday this summer because I could see where was cheapest to fly to. Literally, you have made my summer. " Score: 26]

 ]

In contrast to the subreddit "IAmA", the subreddit with the lowest sum sentiment score was "news". Shocking! :) The post with the comment that had the lowest sum sentiment score is shown below: 

[Subreddit: News
Post: Defense with Dignity: How the Dignity of Violent Resistance Informs the Gun Rights Debate]

The first comment on this post had a score of -60! I'll spare you of posting the two page long comment itself, but here is a little snippet of negativity from it for you: 

[]


- - -

>>>>>>> 807d50f03eace13134043ea550e2af537aadff51
*6-4-15*
