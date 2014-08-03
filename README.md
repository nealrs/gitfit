##GitFit - A pre-commit hook using the Fitbit API

![console screenshot](https://raw.githubusercontent.com/nealrs/gitfit/master/screen.png)

###What it does
Prevents you from committing code unless you've met your primary Fitbit goal for the day.

###Motivation
After coming home from work, I eat dinner in front of my TV and frequently code until ~3am. This is unhealthy. To limit all-nighters, I need to enforce some restrictions. Now, in order to commit code I must first meet one of my Fitbit goals (10,000 steps, 5 miles, or being very active for 30 minutes). If I miss my goal the commit is rejected -- which also means I can't deploy.

_Areas for improvement:_ right now, even if I hit my goal, I can't code after midnight. Then again, that may not be such a bad thing.

###Instructions
0. Install the Python Fitbit API wrapper `pip install fitbit`
1. Make sure hook is executable `chmod u+x pre-commit` & saved to your hooks folder (global or repo level)
2. [Create a new Fitbit app](https://dev.fitbit.com/apps/new) & note down your API keys
3. Get your userid by vising your profile online & noting down the string that comes after `https://www.fitbit.com/user/` (mine is [2SZVTN](https://www.fitbit.com/user/2SZVTN))
4. Make sure your Activities are public here: https://www.fitbit.com/user/profile/privacy
5. Try commiting something
