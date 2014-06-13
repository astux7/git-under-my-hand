Git Under My hand
=================

###Every day Git hints:
Git Setup
--------------
+ Git version
``` git --version ```
+ Set up Git
```
git config --global user.name "your name" 
git config --global user.email "your email"
```
+ Config system to use Git
```
git config --global core.autocrlf input 
git config --global core.safecrlf true
```
Git Routine
--------------
+ Start new project
```git init ```
+ Add all changed files
```git add -A```
+ Local commit the changes
```git commit -m "commit message"```

Git Advanced
--------------

+ Change the last local commit message (not yet pushed to server) <br />
``` git commit --amend -m "new commit message to change the last one" ```

+ Show all local branches use (-a) option; to show all remote branches (-r) <br />
``` git branch -a ```  <br />
``` git branch -r  ```

+ To delete (local or remote) branch <br />
``` git branch -d the_local_branch 
    git push origin :the_remote_branch ```

+ To create a new branch from current checked out branch <br />
``` git checkout -b newbranch ```
