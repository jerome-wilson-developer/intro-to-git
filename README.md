# There are 3 different states of Git. 

# 1. The Working Directory
Everything we are working now is in the state of the Working Directory. This is where all the code in our files and folders are living that we are currently working on.

$ git init >> git -a (show hidden files) = it should now show .git + (master) in green.

# 2. The Staging Area
In order to track specific files, we use git to move those files into the staging area.
$ git add <filename>, or, git add . (adds multiple files) shows up in "red" as an "untracked file". It has not been "Committed and saved yet to the Git Repository (3rd stage) ... >> $git status .

# 3. The .git Repositories
This directory allows us to "Commit and Save" the files we have been tracking to our Git repositories. This is where all our snapshots are stored.

git commit -m (your message about this specific commit). your "message" should start with a present-tense verb ie added, changed, edited, modified. Also, $ git log shows the ID# of each logged file.