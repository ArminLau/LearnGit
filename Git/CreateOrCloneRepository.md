## Create repository
### Create in local pc
* Create a new folder whose name will be the name of new repository, then switch to it
* Execute command below:
```
git init
```
After finish steps above, a new folder named ".git" will be automatically create, never delete or modify it, and the new repository is successfully create in your local pc.
### Create in your Github/Gitlab homepage
* Create a new repository in Github/Gitlab is quite easy, I am sure you can handle this.
  
  
## Clone repository
* Switch to the directory where you want to store repository
* Execute command below(select one of them):
```
git clone git@github.com:ArminLau/LearnGit.git         --SSH protocol
git clone git://github.com/ArminLau/LearnGit.git          --GIT protocol
git clone https://github.com/ArminLau/LearnGit.git      --HTTPS protocol
```



##  Associate local repository with remote repository

If you have created local repository in pc and created the same remote repository in Github, you can associate them with command below:

```
git remote add origin git@github.com:ArminLau/LearnGit.git
```

