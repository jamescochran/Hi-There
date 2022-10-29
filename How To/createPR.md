# Create a PR

Ignore the below. My research at this point tells me that doing a PR on github is a specific feature of GH and can't be done through the git command:

https://stackoverflow.com/questions/34945947/git-request-pull-how-to-create-a-github-pull-request-on-the-command-line/45721044#45721044



---
Once you've created a new branch and made some changes you then probably want to get your changes into master at some point. There are multiple ways to do this but for now I want to do a PR.

So, you're sitting here at your command prompt. Changes have been made. They've been added. You've commited them you your branch. Let's do a PR!

Interestingly I ran into some issues. Do not run the below but instead learn from my mistakes.

`git request-pull v1.0 git@github.com:jamescochran/Hi-There.git master`

The biggest issue I encountered was that I didn't have a version 1.0. 
The second issue is when I looked everyone said don't do it this way use the GUI. :(

In the end I ran:

`git log`

This gave me a lot of information about the commits to my branch and also gave me a long string that was the version number I needed. I was able to modify my command to this which created the PR:

`git request-pull 5e222b1d68a0ec939564b644ca20213583bfe197 https://github.com/jamescochran/Hi-There.git master`

The following is doing a PR, seting the version, setting the repos URL, and telling it to do the PR on master.








This one was a bit of a doozy for me and I leaned on RTFM heavily: 
https://git-scm.com/docs/git-request-pull
