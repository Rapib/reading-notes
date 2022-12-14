# 03 - Revisions and the Cloud

## Version Control

allows users to revert a file / project to a older version, and it also tracks any modifications

> Local Version Control uses your HDD

> Centralized Version Control System (CVCS) uses a server to store all changes and files. It is good for teamwork.

> Distributed Version Control systems (DVCS) is similar to CVCS, but it allows clients to backup / create mirrored repositories. 


## Git

- Git = DVCS
- Commit = save a changed version of the project => Git will creates a snapshot of the file and stores a reference to it
- Mostly relies on local op
- Files in Git can reside in 3 states:  
  - committed (data stored locally)  
  - modified (file is changed, but not committed to the database)  
  - staged (flagged a file's changed version to be committed in the next snapshot)

## Local Git repository:

has 3 components  

1. working Directory: where the actual files reside  
2. Index: area used for staging  
3. Head: points to the most recent commit

### All files in  a working copy of a project file are either  

- tracked (can be modified, unmodified, or staged & part of the most receent snapshot)
- untracked (not in the last snapshot and do not currently reside in the staging area)

*After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited. [^1]


# Git Flow: ACP (Add commit push) 

> git status

What has changed since you last login 

## Add (set file as staged)

> git add FILENAME.extension (add space and files for mulitple files) OR ***`.` for all files - for now in class code-102***

to track a file

> git add *

to track all files in a repo

*After using `git add` commands, files are tracked and staged for committing.

## Commit (to take a snapshot of the staged files)

> git commit –m "your message, what are you changing, log"

Committing a File; commit the changes and record what you did within the commit message

> git commit -a

Committing All Changes *This command commits a snapshot of all modifications to tracked files in the working directory.

## Push (to send your new snapshot of changes to the remote repo)

> git push origin main

push changes to a remote repository (used in class code 102)

> git push origin master

from udemy website

*This command pushes changes from the local “master” branch to the remote repository named “origin”.

*For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local repository. However, these names can be changed by the user.

## Other

> git stash

When you are not ready to commit changes but do not want to lose them either

> git stash apply

When you are ready to continue working on the changes

[^1]: https://blog.udemy.com/git-tutorial-a-comprehensive-guide/  