Git Under My hand
=================

###Every day Git hints:
Git Setup
--------------
+ Git version 
``` git --version ```
+ Git help/about the command
``` git help```
```git help command_name```
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
Git Routine ( practice go to try.github.io)
--------------
+ Start new project 
```git init ```             
+ Checking the status
```git status```
+ Add all changed files or one to staging area
```git add -A```
```git add filename ```
```git add "*.txt"```
+ Local commit the changes
```git commit -m "commit message"```
+ View history
``` git log ```
+ Remove file form git
``` git rm filename```
+ Change the branch or go to specific commit
``` git checkout branchname```
+ Remote add origin 
```git remote add origin https://git@github......git```
+ Push the changes to the server (-u means default branch for the future pushes)
```git push origin branchname```
+ Check remote set ups
``` git remote -v```
+ Get repo changes
```git pull origin branchname```
+ Clone the repo
```git clone https://github.com/blavla...git```
+ Differences from last commit and changes
```git diff HEAD```
+ Differences you staged 
```git diff --staged```
+ Reset/Unstage files
```git reset filename```
+ Undo (reset changes)
```git checkout -- filname```
+ Merge branches ( A branch we merge into B branch)
```git checkout B```
```git merge A```
+ Delete a branch
```git branch -d branchname```
```git push```
+ Clone 
```git clone repo directory```




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
