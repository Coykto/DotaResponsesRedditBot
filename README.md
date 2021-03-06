# Dota Responses Reddit Bot

Bot adding reply comments with links to appropriate responses found on /r/dota2.

*Thanks to /u/iggys_reddit_account the bot is running 24/7.*

![Example](https://i.imgur.com/PAcg57z.png)

The bot replies only for the comments that **are** responses. 

For example:
"Selemene commands" will return a Luna response (like on the screenshot above). 

All the responses are in lowercase in the dictionary, before comparision the comments are parsed to lowercase as well. Dot or exclamation mark ending the comment is ignored.

The bot will try to match a response of the hero that is in the comment's author flair. If it does not find an appropriate one, it takes the one of the first hero that has such a response (alphabetically).

---
# Changelog:

#####2.7
* now hero portraits (flairs) are added before the response
* the bot tries to match the hero response with the hero in the comment's author flair first

#####2.6
* added a few Io and Phoenix responses

#####2.5
* fixed random responses for the "Shitty wizard" line - now it's working properly
* added special treatment for the comments related to "One of my favorites" response
* moved from a dicionary for responses and a list for comment ids to databases

#####2.4
* added random responses for the "Shitty wizard" line (needs testing)

#####2.3:
* added tests
* code refactoring
* added Travis CI and CodeClimate checking

#####2.2:
* code refactoring (renaming variables, deleting unnecessary methods, etc.)
* response in the reply is now an exact quote of the original comment
* added comments

#####2.1:
* bot is now adding the source of the response (e.g. hero name) to the comment *(needs testing)*

#####2.0:
* added Arc Warden responses

#####1.9:
* file paths are now relative to the script file location (using os)
* added dates to logging
* logs are saved in respective files on the server
* fixed a bug with adding same comment a few times in sticky threads that are on the subreddit for a long time (time-saving workaround)

#####1.8:
* change in the main loop of the script - much better efficiency (time)

#####1.7:
* changed reply comment formatting

#####1.6:
* removed keyword triggering as /r/dota2 community did not like it

#####1.5:
* added keywords that trigger the bot: "just do it", "beautiful", "from the ghastly eyrie", "sniper", "ppd", "leafeator", "ur/your brother"
* code refactoring

#####1.4:
* fixed a bug created by 1.2 changes
* changed submissions number in hot to 25
* added more excluded responses

#####1.3:
* removed responses such as "thank you", hero names and item names (anti-spam)

#####1.2:
* accept comments with extra letters added for emphasis

#####1.1:
* one word responses are no longer in the dictionary
* replaced double spaces with single space
* bot is now working with hot submissions

---
##Treeware License
Basically MIT License, but if you use the code (learning or project purposes), you have to plant at least one tree at some future time.
