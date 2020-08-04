# Makers Day 2 - 21st July 2020
#git	#terminal
#commandline #bashcrawl 

_Things I have learned today_

About using Git

The **staging** area (aka index) is a container where **git** collects all changes which will be part of the next commit. If you are editing a versioned file on your local machine, **git** recognises that your file is modified - but it will not be automatically part of your next commit and is therefore **unstaged**.

A **branch** is essentially is a unique set of code changes with a unique name. To begin working on anything new in a project, or to change existing things, you create a branch off the stable **master** branch. 

The term **upstream** and downstream refers to the repository. Generally, **upstream** is from where you clone the repository, and downstream is any project that integrates your work with other works.

A **fork** is a rough copy of a repository. Forking a repository allows you to freely test and debug with changes without affecting the original project. One of the excessive use of forking is to propose changes for bug fixing. 

**git init** - initialises directory as a git repository - it only has to be done once for every repository

You should run git init inside the directory where the files for the project you’re placing under version control are.

If you accidentally initialise a git repo in a folder that shouldn’t be under version control, e.g. by running git init in ~/Desktop, you can revert the change by removing the hidden .git folder:

``` 
rm -rf .git
```

So, the first thing we do when we start a new project is to create a directory, change into it and place it under version control by running git init.

**git add** - adds file to staging area

**git commit** -m ‘First commit’ - committing files to staging area with message, records or snapshots the file permanently in the version history

**git status** - see what’s happening in the repository

**git log** - view all commits made

**git rm** (+ file name) - delete a file

**git checkout**  (+ commit hash from log) - go into a previous commit state or change branch

**git checkout master** - go back to master main branch

**git remote** -v - view git remotes

**git remote set-url origin** git@github.com:_USERNAME_REPOSITORY/.git - change git remote location

**git push -u origin master** - pushes files to GitHub (remote repo)

Then just **git push** can be used going forward

**git pull** - get changes from GitHub to local / working repository and merges changes with what you have already

**git fetch** - get changes from GitHub to local / working repository, but doesn’t merge them with current files

**git clone** (+ GitHub URL) -  copy a GitHub repository

**git merge** - merges one branch history with current branch

_BashCrawl Notes_

ls -F = list files and their file types
Directories end with /
Programs end with *

You can make your shell autocomplete the names of files and
directories by pressing the Tab key after typing the first
few letters.









