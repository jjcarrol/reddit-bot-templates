''' --Reddit Random Quote Reply Bot Template--
    --Created by /u/whaliam--
    --6Ep96ck9@protonmail.com-- '''

# Import required libraries 

import praw
import pdb
import re
import os
import time
import random
import sys
from datetime import datetime

# Create a Reddit API instance

reddit = praw.Reddit(user_agent='<useragent>',
		  client_id='<clientid>',
	          client_secret='<clientsecret>',
		  username='<username>',
		  password='<password>')

# Set up subreddit parameters

subreddit = reddit.subreddit("<subreddit")

# Set up quotes library

quotes = \
[
" <quotation.> ", 
" <quotation.> ",
" <quotation.> ",

]

# Set up comment parameters

for comment in subreddit.stream.comments():
    if re.search("<string you want to locate>",     comment.body, re.IGNORECASE):
        reply = random.choice(quotes)
        comment.reply(reply)

# Cooldown

time.sleep(n) # in seconds
	
