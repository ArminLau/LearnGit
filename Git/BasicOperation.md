# Basic Operation

### Basic concept

First of all, we should know about some concepts of Git:

* Workspace

  The directory in your PC, which includes a subfolder named ".git"

* Staging area

  Normally it exists in index under folder ".git"(.git/index), and it is also known as index

* local repository

  The hidden folder ".git" under workspace

* remote repository

  Corresponding repository in your Github or Gitlab

### Basic command

There are several commands when using Git, the relationship between commands and concepts can be displayed as below:

![git-command](https://github.com/ArminLau/LearnGit/blob/armin/img/git-command.jpg?raw=true)

1. When we create a new text file which we want can be manage by  Git under workspace,  we can use command as below to add it into staging area:

   ```
   git add newFileName
   ```
   
2. After add new file into staging area, we need to execute command as below to submit it to local repository:

   ```
   git commit -m "comment"
   ```
   Someone may be confused, do we repeat 2 steps for all new created file? Of course not, we can add files in one time, just likes

   ```
   git add *	// add all files under current directory into staing area
   git add *.java  // add all *.java files under current directory into staing area
   ```

   And your can execute several "add" commands before execute command "commit". It just like you are shopping in supermarket with a handcart. Each time you take goods from the shelf(create/modify/delete files), you throw them into handcart(add files into staging area). Finally you have to pay the bill for shopping when leaving supermarket(commit and comment "how much you spend on shopping"). 

3. Since you have to execute command "commit" to make sure your modification can be traced by Git. Sometime your modification is not synchronized with the local repository. And you can execute command below to check the difference between workspace and local repository:

   ```
   git status
   ```

   
