# Near-duplicate-detection
#Tweets on a subject are often nearly (but not exactly) duplicates of each other. The file Santa.txt contains a few tweets about Santa Claus, one tweet per line. We will try to detect tweets that we have already seen before.

#(a) Convert each tweet into a dictionary of phrases 
#Write a function called moving_window that takes as input a tweet (that is, a string), and converts it into a bunch of phrases. Each phrase is three con- secutive words in the tweet.
#Return a dictionary whose keys are these phrases, and just set the corresponding values to 1. This dictionary contains all the unique 3-word phrases in the tweet.

#(b) Calculate similarity between two tweets
#To check if one tweet is a near-duplicate of another, we compute their cosine similarity:
#𝑐𝑜𝑠𝑖𝑛𝑒(tweet1,tweet2)=𝑚𝑎𝑡𝑐ℎ𝑒𝑠𝑛1×𝑛2√
#where matches is the number of 3-word phrases in common between the two tweets, and n1 and n2 are the number of phrases in the two tweets respectively.
#Write a function called cosine that takes as input two dictionaries. Each dictionary contains the 3-word phrases from one tweet. Return the cosine similarity between the phrases in the two dictionaries.

#(c) Read in tweets, and output near-duplicates (8 points).
#Read in the tweets in the file Santa.txt. For each tweet, figure out if it is a near-duplicate of any of the previously-seen tweets. We say that the two tweets are near-duplicates if their cosine similarity is greater than 0.5. You should call the functions moving_window and cosine here.
