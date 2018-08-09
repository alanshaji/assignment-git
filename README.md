# Basic Git Commands

### git config
Get and set configuration variables.
Stored in three different places:
 - **/etc/gitconfig file:** Contains values applied to every user on the system.
 - **~/.gitconfig or ~/.config/git/config file*:** Values specific personally to you, the user.
 - **Config file in the Git directory:** Specific to that single repository.

 

### git help <verb>
Getting help about a command.

### git init <Project Name> or git clone <url>
Two ways of getting a git repository.

### git status 
Checking the status of your files.

### git add
Multipurpose command to track new files and stage modified files. 

### git diff
Shows the exact lines added and removed.

### git commit
Permanently saves changes.
To give commit message inline: **git commit -m <"Message">**
To skip the staging area: **git commit -a -m <"Message">**

### git rm
To remove a file from the tracked files or to remove a file from the working directory.

### git log
To view history of commits.

### Undoing Things
To redo a commit: **git commit --amend**
To unstage a staged file: **git reset HEAD <file_name>** 
To unmodify a modified file: **git checkout -- <file_name>**

### git remote
To see which remote servers you have configured.
To add remote repository: **git remote add <shortname> <url>**
To rename: **git remote rename <old_name> <new_name>**

### Getting data from remotes
 - **git fetch <remote>**
 Downloads the data to your local repository. It doesn’t automatically merge it with any of your work. 
 - **git pull**
 Fetches data from the server you originally cloned from and automatically tries to merge it into the code you’re currently working on.

### git push <remote> <branch>
To push data to your remote.

### git remote show <remote>
To see more information about a particular remote.

### git tag
Its a pointer to a specific commit.

### Branching and Merging
To create a new branch: **git branch <branch_name>**
To switch to an existing branch: **git checkout <branch_name>**
To delete a branch: **git branch -d <branch_name>**
To get a simple listing of your current branches: **git branch**
To see the last commit on each branch: **git branch -v**
To see which branches are already merged into the branch you’re on: **git branch --merged**
To push to a remote branch: **git push <remote> <branch>**
To merge to a branch: **git merge <branch>**

### git rebase
The process of moving or combining a sequence of commits to a new base commi

### git cherry-pick <commit-hash>
Choose a commit from one branch and apply it onto another. 

### git reflog
A log which records when the tips of branches and other references were updated in the local repository.

### git rebase -i HEAD~n
To move the changes introduced in a commit into its parent so that you end with one commit out of twos.

