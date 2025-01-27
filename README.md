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
Or pushing existing repo.
```cmd
git push
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

## Collaboration
Fetch changes from the remote repository.
```cmd
git fetch
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
Create a `.gitignore` file and add files/folders to ignore:
  ```cmd
  echo "node_modules/" > .gitignore
```



# Cypress Common commands

## For installing Cypress 
Using npm
```cmd
npm install cypress --save-dev
```

## For Opening Cypress 
Using npx
```cmd
npx cypress open
```


## For checking the Cypress version
Using npx
```cmd
npx cypress --version
```

To make running Cypress easier, add the following to the scripts section of your package.json file:
```cmd
"scripts": {
  "cypress:open": "cypress open",
  "cypress:run": "cypress run"
}
```
Now, you can run:
```cmd
npm run cypress:open
```


## To run Cypress in a headless browser, you can use the following commands:
By default, Cypress uses the Electron browser in headless mode when running tests.

Run in a Specific Browser Headlessly

Run in Headless:
```cmd
npx cypress run --headless
```


## Run Specific Spec File

To run a specific test file, provide the file path:
```cmd
npx cypress run --spec "cypress/e2e/example.cy.js"
```

