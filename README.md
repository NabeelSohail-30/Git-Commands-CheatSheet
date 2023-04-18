# Git-Commands-CheatSheet
Git Commands CheatSheet

# Basic Git Commands
- git init: Initializes a new Git repository in the current directory.
- Syntax: git init

- git add: Adds files or changes to the staging area.
- Syntax: git add <file or directory>

- git commit: Commits changes to the repository with a message.
- Syntax: git commit -m "commit message"

- git status: Shows the status of the working directory.
- Syntax: git status

- git log: Shows the commit history of the repository.
- Syntax: git log

- git diff: Shows the differences between the working directory and the staging area or between two branches.
- Syntax: git diff

- git checkout -b: Creates a new branch and switches to it.
- Syntax: git checkout -b <branch-name>

- git rm: Removes a file from the working directory and staging area.
- Syntax: git rm <file>

- git mv: Renames or moves a file in the working directory and staging area.
- Syntax: git mv <old-path> <new-path>

- git remote add: Adds a remote repository to your local repository.
- Syntax: git remote add <name> <remote-url>


# Branching and Merging
git branch: Lists all branches in the repository.
Syntax: git branch

git branch <branch-name>: Creates a new branch with the specified name.
Syntax: git branch <branch-name>

git checkout: Switches to a different branch.
Syntax: git checkout <branch-name>

git merge: Merges changes from one branch into another.
Syntax: git merge <branch-name>

git branch -d: Deletes a branch.
Syntax: git branch -d <branch-name>

git merge --no-ff: Forces a merge commit to be created when merging a branch, even if the merge is a "fast-forward" merge.
Syntax: git merge --no-ff <branch-name>

git merge --squash: Merges changes from one branch into another, but doesn't create a merge commit.
Syntax: git merge --squash <branch-name>

# Collaboration and Remote Repositories
git clone: Clones a remote repository to your local machine.
Syntax: git clone <remote-url>

git remote: Shows the remote repositories associated with your local repository.
Syntax: git remote

git pull: Fetches changes from a remote repository and merges them into the current branch.
Syntax: git pull <remote> <branch>

git push: Pushes changes to a remote repository.
Syntax: git push <remote> <branch>

git fetch: Fetches changes from a remote repository without merging them into the current branch.
Syntax: git fetch <remote>

git push --force: Forces a push of changes to a remote repository, even if the remote has changes that conflict with the local changes.
Syntax: git push --force <remote> <branch>

git remote -v: Shows the detailed information of remote repositories.
Syntax: git remote -v

# Advanced Git Commands
git rebase: Reapplies changes on top of another base tip.
Syntax: git rebase <base-branch>

git stash: Temporarily stores changes that are not ready to be committed.
Syntax: git stash

git tag: Tags a specific commit with a label.
Syntax: git tag <tag-name>

git reset: Resets the current branch to a specific commit.
Syntax: git reset <commit>

git cherry-pick: Applies a commit from one branch to another.
Syntax: git cherry-pick <commit>

git bisect: Helps find the commit that introduced a bug by performing a binary search through the commit history.
Syntax: git bisect start <bad-commit> <good-commit>

git blame: Shows who last modified each line of a file.
Syntax: git blame <file>

git revert: Reverts a commit by creating a new commit that undoes the changes made by the original commit.
Syntax: git revert <commit>

git reflog: Shows the history of all Git commands that have been executed in the repository.
Syntax: git reflog
