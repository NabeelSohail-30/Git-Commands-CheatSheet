# Git-Commands-CheatSheet
Git Commands CheatSheet


# Git Setup and Initialization
Git Command | Description
----------- | -----------
git config --global user.name “<firstname lastname>” | set a name that is identifiable for credit when review version history
git config --global user.email “<valid-email>” | set an email address that will be associated with each history marker
git config --global color.ui auto | set automatic command line coloring for Git for easy reviewing
git init | initialize an existing directory as a Git repository
git clone <url> | retrieve an entire repository from a hosted location via URL


# Stage and Snapshot
Git Command | Description
----------- | -----------
git status | show modified files in working directory, staged for your next commit
git add <file> | add a file as it looks now to your next commit (stage)
git add -A | adds all new and commited files to the staging area
git add . | adds all new and commited files to the staging area 
git rm <file> | delete the file from project and stage the removal for commit
git rm -r <file> | remove the file or folder
git mv <existing-path> <new-path> | change an existing file path and stage the movegit reset <file> | unstage a file while retaining the changes in working directory
git diff | diff of what is changed but not staged
git diff --staged | diff of what is staged but not yet commited
git commit -m “<descriptive message>” | commit your staged content as a new commit snapshot


# Branch & Merge
Git Command | Description
----------- | -----------
git branch | list your branches. a * will appear next to the currently active branch
git branch -a | List all branches (local and remote)
git branch <branch-name> | create a new branch at the current commit
git branch -d <branch name> | Delete a branch
git branch -m <old branch name> <new branch name> | Rename a local branch
git merge <alias>/<branch> | merge a remote branch into your current branch to bring it up to date
git merge <branch name> | Merge a branch into the active branch
git merge <source branch> <target branch> | Merge a branch into a target branch
git merge <branch> | merge the specified branch’s history into the current one
git merge --no-ff <branch-name> | Forces a merge commit to be created when merging a branch, even if the merge is a "fast-forward" merge
git merge --squash <branch-name> | Merges changes from one branch into another, but doesn't create a merge commit
git checkout -b <branch name> | Create a new branch and switch to it
git checkout -b <branch name>origin/<branch name> | Clone a remote branch and switch to it
git checkout | switch to another branch and check it out into your working directory
git checkout <branch name> | Switch to a branch
git checkout - | Switch to the branch last checked out
git checkout -- <file-name.txt> | Discard changes to a file


# Inspection & Comparison
Git Command | Description
----------- | -----------
git log | show all commits in the current branch’s history
git log branchB..branchA | show the commits on branchA that are not on branchB
git log --follow <file> | show the commits that changed file, even across renames
git log --stat -M | show all commit logs with indication of any paths that moved
git diff branchB...branchA | show the diff of what is in branchA that is not in branchB
git show <SHA> | show any object in Git in human-readable format


# Collaboration and Remote Repositories
Git Command | Description
----------- | -----------
git remote | Shows the remote repositories associated with your local repository
git remote -v | Shows the detailed information of remote repositories
git remote add origin <url> | Add a remote repository
git remote set-url origin <url> | Set a repository's origin branch to SSH
git remote add <alias> <url> | add a git URL as an alias
git fetch <alias> | fetch down all the branches from that Git remote
git fetch <remote> | Fetches changes from a remote repository without merging them into the current branch
git push <alias> <branch> | Transmit local branch commits to the remote repository branch
git push origin <branch name> | Push a branch to your remote repository
git push -u origin <branch name> | Push changes to remote repository (and remember the branch)
git push | Push changes to remote repository (remembered branch)
git push origin --delete <branch name> | Delete a remote branch
git push <remote> <branch> | Pushes changes to a remote repository
git push --force <remote> <branch> | Forces a push of changes to a remote repository, even if the remote has changes that conflict with the local changes
git pull | fetch and merge any commits from the tracking remote branch
git pull <remote> <branch> | Fetches changes from a remote repository and merges them into the current branch
git pull origin <branch name> | Pull changes from remote repository


# Advanced Commands
Git Command | Description
----------- | -----------
git rebase <branch> | apply any commits of current branch ahead of specified one
git reset --hard <commit> | clear staging area, rewrite working tree from specified commit
git tag <tag-name> | Tags a specific commit with a label
git reset <commit> | Resets the current branch to a specific commit
git cherry-pick <commit> | Applies a commit from one branch to another
git bisect start <bad-commit> <good-commit> | Helps find the commit that introduced a bug by performing a binary search through the commit history
git blame <file> | Shows who last modified each line of a file
git revert <commit> | Reverts a commit by creating a new commit that undoes the changes made by the original commit
git reflog | Shows the history of all Git commands that have been executed in the repository

  
# Temporary Commits
Git Command | Description
----------- | -----------
git stash | Save modified and staged changes
git stash clear | Remove all stashed entries
git stash list | list stack-order of stashed file changes
git stash pop | write working from top of stash stack
git stash drop | discard the changes from top of stash stack
