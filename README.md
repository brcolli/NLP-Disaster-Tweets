# NLP-Disaster-Tweets
Kaggle NLP Disaster Tweets contest 2020

## Clone Instructions
Open your bash terminal and navigate to the directory where you wish to place your repo. Use the *cd* command to navigate directories, like the example below.
```
$ cd C:\Users\$USER\Documents
```

Clone the repository with the following command:
```
$ git clone https://github.com/brcolli/NLP-Disaster-Tweets.git
```

This will create a new directory called *NLP-Disaster-Tweets*. From this directory, if your git is properly set up, you should be able to push and pull to the repo.

## Committing your changes
Before you can push your changes to the server, you must *commit* your changes. This is how you tell git which changes you want to push. There are two steps:
the first is staging the changes so git knows which files should be pushed, and the second is packaging them into a commit with a commit message.
Use the following commands to add and commit your changes:
```
$ git add -A
$ git commit -m "My commit message"
```

Once you have added and committed your changes, you are ready to push and pull.

## Pushing and Pulling
**_Pushing_** means to push your local changes (changes you made on your computer to the repo) to the remote repo (the version saved on the server).
The format is as follows:
```
$ git push REMOTE BRANCH
```
For our purposes, REMOTE will always be *origin* and BRANCH will always be *master*. Therefore, the command to push to the server will be:
```
$ git push origin master
```

**_Pulling_** means to bring in the version that is saved on the server. This will allow you to bring in any changes someone else has made and pushed.
Git will attempt to merge any files and changes, such that you don't lose your own local changes. If there are merge conflicts, git will tell you before it overwrites anything.
The format is as follows:
```
$ git pull REMOTE BRANCH
```
For our purposes, REMOTE will always be *origin* and BRANCH will always be *master*. Therefore, the command to pull from the server will be:
```
$ git pull origin master
```

A typical workflow would be to start your coding session by pulling in any changes made to the server, then make any changes you wish, then add your changes, commit your changes,
and finally push your changes.
```
$ git pull origin master
.......
DO CODING
.......
$ git add -A
$ git commit -m "I did some coding!"
$ git push origin master
```

**Note:** If the repo was changed while you were coding or making changes, you will need to pull those changes in before you push, BUT AFTER you commit. This would look like so:
```
$ git pull origin master
.......
DO CODING
.......
$ git add -A
$ git commit -m "I did some coding!"
# git pull origin master
$ git push origin master
```

Do not be afraid to make mistakes! Git has version control history, anything you break can probably be fixed. Happy coding~
