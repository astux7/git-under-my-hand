Git Under My hand (https://www.atlassian.com/git/tutorials)
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
Define the author name to be used for all commits by the current user.
```
git config --global user.name "your name" ```

Define the author email to be used for all commits by the current user.
```
git config --global user.email "your email"
```
+ Config system to use Git
```
git config --global core.autocrlf input 
git config --global core.safecrlf true
```
Select your favorite text editor
```git config --global core.editor vim```

Git Routine ( practice go to try.github.io)
--------------
+ Start new project 
```git init```

Running this command will create a new folder called <directory containing nothing but the .git subdirectory.
  
```git init <directory>```

Initialize an empty Git repository, but omit the working directory. Shared repositories should always be created with the --bare flag .The --bare flag creates a repository that doesn’t have a working directory, making it impossible to edit files and commit changes in that repository. 

```git init --bare <directory>```

+ Checking the status
```git status```
+ Add all changed files or one to staging area
```git add -A```
```git add filename ```
```git add "*.txt"```
Begin an interactive staging session that lets you choose portions of a file to add to the next commit. This will present you with a chunk of changes and prompt you for a command. Use y to stage the chunk, n to ignore the chunk, s to split it into smaller chunks, e to manually edit the chunk, and q to exit.
```git add -p```
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
+ go to specific commit 
```git log --oneline```
```git checkout a123fee hello.py```
+ revert (safe way)
```git revert <commit>```
to go back use
```git checkout HEAD hello.py```
+ Reset When you undo with git reset(and the commits are no longer referenced by any ref or the reflog), there is no way to retrieve the original copy—it is a permanent undo. 
```git reset file```
reset staging area 
```git reset --hard```
+ git log all history (next space , exit q)
```git log -n <limit>```
specific file information
```git log filename```
commits seach by author 
```git log --author="<pattern>"```
or pattern
```git log --grep="<pattern>"```
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
+ Clean directory
The git clean command removes untracked files from your working directory. 
``` git clean -n ```
shows which files are going to be remove

force remove files
```git clean -f```

force remove files and dir 
```git clean -xf```
