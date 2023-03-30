# Git 

Git is a distributed version control software that basically allows multiple people to work in parallel and it saves a history of all changes made. 
We advise to use git in your group work as git will help ensure that there are no code conflicts as well as allow developers the ability to revert files or entire projects back to a previous version of their code.
## Prerequistion 
Install [GIT](https://education.github.com/git-cheat-sheet-education.pdf).
Create a [Github](www.github.com) or [GitLab](www.gitlab.com) Account if you not already have one 

## Usage 
In this section the basic usage of git commandline tool is described. 
If you do not want to use GIT via command line multiple IDS offer a git integration providing a UI for the steps described below (e.g.,
[Plugin for Visual Code](https://code.visualstudio.com/docs/sourcecontrol/overview))


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

## Small Tutorial on Git 
If you want to test / try git follow the tutorial [here](https://towardsdatascience.com/an-easy-beginners-guide-to-git-2d5a99682a4c)

## Further 
Further Calls to github can be found on the [Cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf).