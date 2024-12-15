# GIT and GIT HUB

some basic GIT commands

## Baisc operations 
- `git init` create a new Git repository in your project folder.
- `git add .` Add all changes to the staging area.
- `git commit -m "commit comment" -m "commit description" ` Save changes to the repo with message and description.

## Branching 
- `git branch` Create a new branch.
- `git branch <branch_name >` Create a new branch.
- `git checkout <branch_name>` Switch to a specific branch.
- `git mege <branch_name>` Merge a branch into current brnach.

## Remote Repositories
- `git remote add origin <url>` Link to a remote repository.
- `git push origin <branch>` Push changes to the remote repository.
- `git pull origin <branch>` Fetch and mergr changes from the remote repository.

## Status and log
- `git status` Show the state of the working directory and staging area.
- `git log` Show the commit history.

## Cloning 
- `git clone <url>` Copy a remote repository to the local machine.

## viewing and inspecting 
- `git diff` Show changes between commits, working directory, and staging area
- `git diff <branch_name>` Compare the current branch with another branch
- `git show <commit_hash>` Show detailed information about a specific commit
- `git log --oneline` Compact view of the commit history.
- `git log --graph --all` View the commit graph across all branches.

## Undoing changes
- `git reset <file>` Unstage a file from the staging area.
- `git reset --hard` Discard all changes in the working directory and staging area.
- `git reset <commit_hash>` Move the Head pointer to a specific commit (keeps changes in the working Directory).
- `git revert <commit_hash>` Undo a specific commit by creating a new commit.

## Tagging
- `git tag <tag_name>`: Create a lightweight tag.
- `git tag -a <tag_name>` -m "Message": Create an annotated tag.
- `git push origin <tag_name>`: Push a tag to the remote repository.
- `git tag -d <tag_name>`: Delete a tag locally.

## Stashing
- `git stash`: Save uncommitted changes for later.
- `git stash list`: View stashed changes.
- `git stash apply`: Reapply the most recent stash.
- `git stash pop`: Reapply and remove the most recent stash.
- `git stash drop`: Remove a specific stash.

## Remote Repository Management
- `git remote -v`: View remote repositories linked to your local repo.
- `git remote remove <name>`: Remove a remote repository.
- `git fetch <remote>`: Fetch changes from the remote repository without merging.
- `git cherry-pick <commit_hash>`: Apply changes from a specific commit to the current branch.

## Branch Management
- `git branch -d <branch_name>`: Delete a branch locally.
- `git branch -D <branch_name>`: Force-delete a branch locally.
- `git push origin --delete <branch_name>`: Delete a remote branch.
- `git checkout -b <branch_name>`: Create and switch to a new branch.

## Advance debugging 
- `git blame <file>`: Show who made each change to a file.
- `git reflog`: View the history of HEAD changes.
- `git clean -f`: Remove untracked files in the working directory.
- `git bisect`: Find the commit that introduced a bug using binary search.

## some useful question and answers

If you want to look at or test a specific commit without altering your current branch:

> `git checkout <commit_hash>`

Creating a New Branch at a Specific Commit

> `git checkout -b <new_branch_name> <commit_hash>`
