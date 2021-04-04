# Branch Management

### Basic Command

```
git branch -r		#check all remote branches

git branch		#check all local branches

git branch -a		#check all branches from local and remote

git checkout branch_name		#switch to a branch

git push origin -d branch_name		#delete a remote branch

git branch -d branch_name		#delete a local branch

git remote prune origin		#delect branches that have been deleted in remote branches

git remote show origin		#check the relationship between remote branches and local branches
```



### scenarios

> Scene One:   synchronize local branch with remote branch

* execute  `git branch -a`  to check the difference between local branch and remote branch

* execute  `git fetch`  to update local repository from remote repository, after which it is able to view new remote branches

* execute  `git checkout -b remote_branch_name`  to fetch remote branch to local branch

  

> Scene Two:   create a new branch "temp" from master to develop new function

* navigate to the directory where you want to save project, execute  `git clone git@github.com:ArminLau/LearnGit.git`  to fetch newest code from master

* execute `git checkout -b temp` to create and switch to new branch "temp"

* develop new function under branch "temp", remember to add and commit new files

* execute `git checkout master` to switch back to master branch

* execute `git merge temp` to merge code that created by branch temp to master branch

* execute `git push -u origin master` to push code to remote repository

  

> Scene Three:  need to update code of branch "dev" when the code of master branch changes

* execute `git checkout master` to switch to master branch

* execute `git pull` to fetch newest code for master branch

* execute  `git checkout dev` to switch back to dev branch

* execute  `git merge master` to merge new code of master branch to current branch dev

* execute `git push -u origin dev` to push code to remote repository

  