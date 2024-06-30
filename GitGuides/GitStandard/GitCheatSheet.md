# Git Cheat Sheet

## Basic Git Commands

- `git init`: Initialize a new Git repository.
- `git clone <repository>`: Clone a remote repository to your local machine.
- `git add <file>`: Add a file to the staging area.
- `git commit -m "<message>"`: Commit changes to the repository with a descriptive message.
- `git status`: View the status of your repository.
- `git log`: View the commit history.

## Branching and Merging

- `git branch`: List all branches in the repository.
- `git branch <branch-name>`: Create a new branch.
- `git checkout <branch-name>`: Switch to a different branch.
- `git merge <branch-name>`: Merge changes from a different branch into the current branch.

## Remote Repositories

- `git remote add <name> <url>`: Add a remote repository.
- `git push <remote> <branch>`: Push local changes to a remote repository.
- `git pull <remote> <branch>`: Pull changes from a remote repository to your local machine.

## Undoing Changes

- `git reset <commit>`: Undo commits and move the HEAD pointer.
- `git revert <commit>`: Create a new commit that undoes the changes made in a previous commit.
- `git checkout -- <file>`: Discard changes made to a file.

## Miscellaneous

- `git diff`: Show the differences between the working directory and the staging area.
- `git blame <file>`: Show who made changes to a file and when.

Remember to always consult the official Git documentation for more detailed information.
