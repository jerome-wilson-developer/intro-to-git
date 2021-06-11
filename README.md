# Intro to "The 3 Different Stages of Git"
 There are 3 different states of Git which have 3 different purposes for getting your code you are creating on your IDE to the world wide web where anybody can see your work. 

# 1. The Working Directory
Everything we are working now is in the state of the Working Directory. This is where all the code in our files and folders are living that we are currently working on.

$ git init >> git -a (show hidden files) = it should now show .git + (master) in green.

# 2. The Staging Area
In order to track specific files, we use git to move those files into the staging area.
$ git add <filename>, or, git add . (adds multiple files) shows up in "red" as an "untracked file". It has not been "Committed and saved yet to the Git Repository (3rd stage) ... >> $git status .

# 3. The .git Repositories
This directory allows us to "Commit and Save" the files we have been tracking to our Git repositories. This is where all our snapshots are stored.

git commit -m (your message about this specific commit). your "message" should start with a present-tense verb ie added, changed, edited, modified. Also, $ git log shows the ID# of each logged file.

# GIT COMMANDS AND WHAT THEY DO

mkdir = Create a new directory for your project.

cd <folder name> = Change a directory into your project folder.

git init = Initialize a Git repository to begin tracking your project.

git status = Check the current status of your progress and actions.

git add <file name> = Add a file name to staging to be committed to the repository.

git add . = Add all modified files to staging to be commited to the repository.

git commit -m "message ... starts with a present tense verb" = This git command commits the files during staging that will be uploaded to the repository.


# Removing files and folders from the staging area !!!
Example: cd intro-to-git  >>>  touch remove-file.txt  >>>   ls (shows all files inside this folder)  >>>  git status [(shows any files that are NOT currently being tracked)  >>>  $ git status (On branch master  Untracked files: (use "git add <file>..." to include in what will be committed) remove-file.txt nothing added to commit but untracked files present (use "git add" to track)]  >>>  git add remove-file.txt >>>  $ git status [On branch master. Changes to be committed: (use "git restore --staged <file>..." to unstage) new file: remove-file.txt  >>>  git add remove-file-2  >>>  git status  >>>  git commit -m "added file remove-file-2"  >>>  git status  >>>  