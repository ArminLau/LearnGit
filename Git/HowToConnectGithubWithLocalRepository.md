## How to connect Github with local repository?

As we know, everyone is allowed to clone or download these public repository from Github. But it is not accessible for everyone to update public repository, else it is unsafe. 

Github supports two methods for authentication: **HTTPS & SSH**

### HTTPS

When you are trying to push local repository to remote repository, there will be pop-ups requiring you to input your username and password. Only by providing correct info, can you push successfully.

#### How to set HTTPS as authentication method?

```
git remote set-url origin https://github.com/ArminLau/LearnGit.git
```

HTTPS authentication is easy, but it is annoying for you have to input username/password each time you want to push



### SSH

SSH is more convenient. Once you have configured successfully, you do not need to provide your username/password when pushing.

#### How to set SSH as authentication method?

```
git remote set-url origin git@github.com:ArminLau/LearnGit.git
```

However, it is only the precondition.

> **Microsoft Windows:**

* Step 1

  Switch to your home directory to check whether there is a directory named ".ssh" that includes id_rsa and id_rsa.pub or not. If it exists, it seems that you have configured SSH Key previously, just ignore step2.

* Step 2

  Execute command under your home directory(open Git Bash):

  ```
  ssh-keygen -t rsa -C "youremail@example.com"
  ```
  If operation is done, there will be a new folder named ".ssh" under home page, which includes id_rsa and id_rsa.pub
  
* Step 3

  Sign in Github, navigate to <kbd>Account Settings</kbd>, select <kbd>SSH and GPG keys</kbd>, click on <kbd>Add SSH Key</kbd>, input random titile, then paste the content of id_rsa.pub into "Key textarea",  finally click on <kbd>Add Key</kbd>
  
  ![](https://github.com/ArminLau/LearnGit/blob/main/img/img_SSH_Configuration.JPG)
  
  And now configuration is finished.
