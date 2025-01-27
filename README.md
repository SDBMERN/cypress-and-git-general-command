# Git and GitHub Command Guide

## Configuration
Set username.
```cmd
 git config --global user.name "Your Name"
 ```
Set user email.
```cmd
git config --global user.email "your_email@example.com"
```
Check configurations.
```cmd
git config --list
```

## Repository Initialization
Initialize a new repository.
```cmd
git init
```

## Working with Remote Repositories
Clone a repository.
```cmd
git clone <repository-url>
```
Add a remote repository.
```cmd
git remote add origin <repository-url>
```
Show remote repositories.
```cmd
git remote -v
```

## Staging and Committing Changes
Check the status of the repository.
```cmd
git status
```
Add specific files to the staging area.
```cmd
git add <file>
```
Add all files to the staging area.
```cmd
git add .
```
Commit changes with a message.
```cmd
git commit -m "Your commit message"
```

## Branching
Create a new branch.
```cmd
git branch <branch-name>
```
Switch to a branch.
```cmd
git checkout <branch-name>
```
Create and switch to a new branch.
```cmd
git checkout -b <branch-name>
```
List all branches.
```cmd
git branch
```

## Merging
Merge a branch into the current branch.
```cmd
git merge <branch-name>
```

## Pushing and Pulling
Push changes to a remote repository.
```cmd
git push origin <branch-name>
```
Pull changes from a remote repository.
```cmd
git pull origin <branch-name>
```

## Log and History
View commit history.
```cmd
git log
```
View a concise commit history.
```cmd
git log --oneline
```

## Undo Changes
Undo all unstaged changes.
```cmd
git checkout -- <file>
```
Unstage a file from the staging area.
```cmd
git reset <file>
```
Reset to the last commit (soft, keeps changes).
```cmd
git reset --soft HEAD~1
```
Reset to the last commit (hard, removes changes).
```cmd
git reset --hard HEAD~1
```

## Tags
Create a tag.
```cmd
git tag <tag-name>
```
List all tags.
```cmd
git tag
```
Push a tag to the remote repository.
```cmd
git push origin <tag-name>
```

## Stashing
Save changes temporarily.
```cmd
git stash
```
Apply the last stashed changes.
```cmd
git stash apply
```
List all stashes.
```cmd
git stash list
```

## Collaboration
Fetch changes from the remote repository.
```cmd
git fetch
```
Rebase your branch with the main branch.
```cmd
git rebase main
```

## Delete Branches
Delete a local branch.
```cmd
git branch -d <branch-name>
```
Delete a remote branch.
```cmd
git push origin --delete <branch-name>
```

## Ignoring Files
- Create a `.gitignore` file and add files/folders to ignore:
  ```bash
  echo "node_modules/" > .gitignore
