# Git and GitHub Command Guide

## Configuration
- `git config --global user.name "Your Name"`: Set username.
- `git config --global user.email "your_email@example.com"`: Set email.
- `git config --list`: Check configurations.

## Repository Initialization
- `git init`: Initialize a new repository.

## Working with Remote Repositories
- `git clone <repository-url>`: Clone a repository.
- `git remote add origin <repository-url>`: Add a remote repository.
- `git remote -v`: Show remote repositories.

## Staging and Committing Changes
- `git status`: Check the status of the repository.
- `git add <file>`: Add specific files to the staging area.
- `git add .`: Add all files to the staging area.
- `git commit -m "Your commit message"`: Commit changes with a message.

## Branching
- `git branch <branch-name>`: Create a new branch.
- `git checkout <branch-name>`: Switch to a branch.
- `git checkout -b <branch-name>`: Create and switch to a new branch.
- `git branch`: List all branches.

## Merging
- `git merge <branch-name>`: Merge a branch into the current branch.

## Pushing and Pulling
- `git push origin <branch-name>`: Push changes to a remote repository.
- `git pull origin <branch-name>`: Pull changes from a remote repository.

## Log and History
- `git log`: View commit history.
- `git log --oneline`: View a concise commit history.

## Undo Changes
- `git checkout -- <file>`: Undo all unstaged changes.
- `git reset <file>`: Unstage a file from the staging area.
- `git reset --soft HEAD~1`: Reset to the last commit (soft, keeps changes).
- `git reset --hard HEAD~1`: Reset to the last commit (hard, removes changes).

## Tags
- `git tag <tag-name>`: Create a tag.
- `git tag`: List all tags.
- `git push origin <tag-name>`: Push a tag to the remote repository.

## Stashing
- `git stash`: Save changes temporarily.
- `git stash apply`: Apply the last stashed changes.
- `git stash list`: List all stashes.

## Collaboration
- `git fetch`: Fetch changes from the remote repository.
- `git rebase main`: Rebase your branch with the main branch.

## Delete Branches
- `git branch -d <branch-name>`: Delete a local branch.
- `git push origin --delete <branch-name>`: Delete a remote branch.

## Ignoring Files
- Create a `.gitignore` file and add files/folders to ignore:
  ```bash
  echo "node_modules/" > .gitignore
