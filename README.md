# GIT Notes
Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. 
If the file has not changed, Git only stores a reference to the already-stored identical version of it.

Git is like an automatic storage unit where you can pull from as needed. 
Git makes it nearly impossible to lose any files because once the file is snapshot it'll be tracked once after its pushed.

#States

Files in Git can reside in three main states: committed, modified and staged.

##Committed

Data is securely stored in a local database

##Modified

File has been changed but not committed to the database

##Staged

Flagged a file’s changed version to be committed in the next snapshot

# History of Git

Git traces its roots to the open source software project Linux kernel. Developers of this project began using a DVCS called BitKeeper in 2002.
In 2005, many of these developers stopped using this DVCS due to tension between the Linux kernel community and the company behind BitKeeper’s and the eventual revocation of the DVCS’ gratis status. 
Subsequently, Linus Torvalds, the chief architect of the Linux kernel, began creating Git. With the intention of creating a DVCS with a workflow design similar to that of BitKeeper, which was also fast, Git allowed for non-linear development via multiple branches, could support large projects, possessed strong mechanisms preventing corruption, and had a simple design. 
Since its inception in 2005, Git has become one of the most utilized Version Control Systems in the world.

# Identity Setting

## After installing Git, users should immediately set the user name and email address, which will be used for every Git commit.

Type the following into Terminal or Command Line:

git config --global user.name "Jane Smith"

git config --global user.email "example@email.com"

To confirm that you have the correct settings, enter the following command:

git config --global user.name (should return Jane Smith)

git config --global user.email (should return example@email.com)
*By using the –global option, these Git settings apply to anything on the system. 
To use different identity settings for a specific project, change the working directory to the desired local Git repository and repeat the steps above without using –global.

It's important to make sure that your username and email are displayed properly in the terminal otherwise whenever you want to pull from a repo, your terminal can't display it because it wont know where to pull the file from.
 # Setting up git repository
 
 To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

Switch to the target project’s directory
Example:

$ cd test (cd = change directory)
Use the git init command
$ git init

to start tracking these repository files, perform an initial commit by typing the following:
$ git add *.c
$ git add LICENSE
$ git commit -m “any message here”

# Cloning
 git clone https://github.com/test
 
 git clone https://github.com/test mydirectory
 
#  Check File Status
  git status
 
 git add filename (single file)/ git add * (all files)
 
 git commit -m “made change x,y,z”
 
 git push origin master
 
