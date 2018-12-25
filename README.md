# instagrowth
Grow your instagram follows

What this bot does?
- Open a browser and login with your credentials
- For every hashtag in the hashtag list, it will open the page and click the first picture to open it
- It will then like, follow, comment and move to the next picture, in a 200 iterations loop (number can be adjusted)
- Saves a list with all the users you followed using the bot

## Setup 
You’ll need Python (I’m using Python 3.7), Selenium, a browser (such as Chrome) and an Instagram account!

1. Download chrome driver http://chromedriver.chromium.org/
2. Set the path to chromedriver_path in loginbot.py
3. Enter your username and password in loginbot.py
4. Run the loginbot.py 
5. Add hashtags in the hashtag_list of interact-bot.py. 
6. One thing to note, if you run it for the first time, you still don’t have a file with the users you followed, so you can simply create prev_user_list as an empty list.
7. Once you run it once, it will save a csv file with a timestamp with the users it followed. That file will serve as the prev_user_list on your second run. Simple and easy to keep track of what the bot does.
8. Update with the latest timestamp on the following runs and you get yourself a series of csv backlogs for every run of the bot.
