# Git 

## Prerequistion 
Install [GIT] [https://education.github.com/git-cheat-sheet-education.pdf].
Create a [Github][www.github.com] or [GitLab][www.gitlab.com] Account if you not already have one 

## Usage 
In this section the basic usage of git commandline tool is described. 
If you do not want to use GIT via command line multiple IDS offer a git integration providing a UI for the steps described below (e.g.,
[Plugin for Visual Code][https://code.visualstudio.com/docs/sourcecontrol/overview])


A) Create new Project. 
Go to local project folder. 
```
git init
```
B) Clone a Project from Github. 
```
git clone [path]
```

C) Add changes made to a project. 
```
git add .
git commit -m 'Commit Message' # should describe the changes you made
```
Push it onto gitlab/github. 
```
git push 
```
D) Add branch. 
If you collaborate on a project (2+ developer) it make sense to work on different branches (i.e., different versions of the same code). 
A new branch can be added with: 
```
git checkout -b [branchname]
```
Switching between branches : 
```
git checkout [branchname]
```
If you want to merge your code into one branch (or the main branch ):
```
git merge []  []
```
In case of merge conflicts (e.g., both developer made changes the same code lines ), merge will trigger a code comparison. 

## Further 
Further Calls to github can be found on the [Cheatsheet][https://education.github.com/git-cheat-sheet-education.pdf].