# David SCTP2 Mod 3.2 Assignment

## What is GitHub Authentication and what methods are available to be implemented?
> GitHub Authentication is a mechanism that allows users to securely access GitHub's services and resources.
It verifies the identity of users and ensures that only authorized individuals can perform actions like pushing code, 
creating repositories, or interacting with APIs.
> 
>The most common methods include : 
> - username and password authentication
> - OAuth authentication
> - personal access tokens

## Github Commands

###

#### **Setup & Init**

| Git | Description |
| ------ | ------ |
| git init | initialize an existing directory as a Git repository |
| git clone [url] | retrieve an entire repository from a hosted location via URL |

#### **Stage & Snapshot**

| Git | Description |
| ------ | ------ |
| git status | show modified files in working directory, staged for your next commit |
| git add [file] | add a file as it looks now to your next commit (stage) |
| git reset [file] | unstage a file while retaining the changes in working directory |
| git diff | diff of what is changed but not staged |
| git diff --staged | diff of what is staged but not yet commited |
| git commit -m "remarks" | commit your staged content as a new commit snapshot |

#### **Branch & Merge**

| Git | Description |
| ------ | ------ |
| git branch | list your branches. a * will appear next to the currently active branch |
| git branch [branch-name] | create a new branch at the current commit |
| git checkout | switch to another branch and check it out into your working directory |
| git merge [branch] | merge the specified branch’s history into the current one |
| git log | show all commits in the current branch’s history |


#### **Inspect & Compare**

| Git | Description |
| ------ | ------ |
| git log branchB..branchA | show the commits on branchA that are not on branchB |
| git log --follow [file] | show the commits that changed file, even across renames |
| git diff branchB...branchA | show the diff of what is in branchA that is not in branchB |
| git show [SHA] | show any object in Git in human-readable format |


#### **Share & Update**

| Git | Description |
| ------ | ------ |
| git remote add [alias] [url] | add a git URL as an alias |
| git fetch [alias] | fetch down all the branches from that Git remote |
| git merge [alias]/[branch] | merge a remote branch into your current branch to bring it up to date |
| git push [alias] [branch] | Transmit local branch commits to the remote repository branch | 
| git pull | fetch and merge any commits from the tracking remote branch |


#### **Share & Update**

| Git | Description |
| ------ | ------ |
| git rm [file] | delete the file from project and stage the removal for commit |
| git mv [existing-path] [new-path] | change an existing file path and stage the move |
| git log --stat -M | show all commit logs with indication of any paths that moved |


#### **Temporary Commits**

| Git | Description |
| ------ | ------ |
| git stash | Save modified and staged changes |
| git stash list | list stack-order of stashed file changes |
| git stash pop | write working from top of stash stack |
| git stash drop | discard the changes from top of stash stack |

#### **Rewrite History**

| Git | Description |
| ------ | ------ |
| git rebase [branch] | apply any commits of current branch ahead of specified one |
| git reset --hard [commit] | clear staging area, rewrite working tree from specified commit |

#### **Ignoring Patterns**

- Preventing unintentional staging or commiting of files

***logs/***

****.notes***

***pattern***/*
> Save a file with desired paterns as .gitignore with either direct string
matches or wildcard globs.

- git config --global core.excludesfile [file]
> system wide ignore patern for all local repositories


## Most used Github commands in the real project
- git clone
> This commands allows us to create a local copy of a remote Git repository on our local computer
- git add
> It important because it stages change for commit
- git commit
> To commit our staged content, it creates a permanent snapshot of the staged changes in our repository
- git push
> Important to transmit local branch commits to the remote repository