# Git?
## Git is a DVCS that stores data in a file system made up of snapshots. 
## Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. 
## If the file has not changed, Git only stores a reference to the already-stored identical version of it.

#States

Files in Git can reside in three main states: 
*committed* (Data is securely stored in a local database)
 *modified* (File has been changed but not committed to the database)
 *staged* (Flagged a file’s changed version to be committed in the next snapshot)
 
 
 # Initial Customization
## After making sure Git has been installed, you should perform some customization steps, which should only need to be completed once on any machine. 
## To change settings, you can repeat these steps.

# Identity Setting

After installing Git, users should immediately set the user name and email address, which will be used for every Git commit.

Type the following into Terminal or Command Line:

**git config --global user.name "Jane Smith"**

**git config --global user.email "example@email.com"**
To confirm that you have the correct settings, enter the following command:

**git config --global user.name (should return Jane Smith)**

**git config --global user.email (should return example@email.com)**

# Importing
 **cd test (cd = change directory)**
 **git init**
 
 # To start tracking these repository files, perform an initial commit by typing the following:
*git add *.c
 git add LICENSE
 git commit -m “any message here”*
 
 # Cloning
You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:
**git clone https://github.com/test**
To clone a repository into a directory with another name of your choosing, use the following command format:

**git clone https://github.com/test mydirectory**

# Saving changes
*Tracked (Saved) Untrackked (Unsaved)*

## Single File- git add filename

git status

On branch master

Changes to be committed:

  (use "git reset HEAD ..." to unstage)
  
  ## Committ
  git commit -a
  
  ## Push
  git push origin master
  
 
