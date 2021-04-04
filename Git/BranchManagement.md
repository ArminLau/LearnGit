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

> Scene One:	synchronize local branch with remote branch

* execute  `git branch -a`  to check the difference between local branch and remote branch

* execute  `git fetch`  to update local repository from remote repository, after which it is able to view new remote branches

* execute  `git checkout -b remote_branch_name`  to fetch remote branch to local branch

  