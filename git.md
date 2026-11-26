# GIT COMMANDS CHEAT SHEET

## Installation and Configuration

`git --version` – Check Git version.

`git config --global user.name "Name"` – Set Git username.

`git config --global user.email "email"` – Set Git email.

`git config --list` – Display Git configuration.

## Repository Creation

`git init` – Initialize a new local repository.

`git clone URL` – Clone a remote repository.

`git status` – Check repository status.

`git remote -v` – Display remote repository URLs.

`git remote add origin URL` – Connect local repository to GitHub.

`git remote set-url origin URL` – Change remote repository URL.

## File Operations

`git add filename` – Stage a specific file.

`git add .` – Stage all changes.

`git commit -m "message"` – Save staged changes.

`git commit -am "message"` – Stage and commit modifications to tracked files.

`git diff` – Display unstaged changes.

`git rm filename` – Delete a file and stage its removal.

## GitHub Operations

`git push origin main` – Upload commits to GitHub.

`git push -u origin main` – Push main and set upstream tracking.

`git pull origin main` – Download and integrate remote changes.

`git fetch origin` – Download remote changes without merging.

## Branching

`git branch` – List local branches.

`git branch feature` – Create a new branch.

`git checkout feature` – Switch to feature branch.

`git checkout -b feature` – Create and switch to a new branch.

`git switch main` – Switch to main branch.

`git branch -d feature` – Delete a merged branch.

## Merging

`git merge feature` – Merge feature branch into current branch.

`git merge main` – Merge main into current branch.

## History

`git log` – Display commit history.

`git log --oneline` – Display compact commit history.

`git log --oneline --all --graph` – Display graphical history of all branches.

## Undo and Restore

`git restore filename` – Discard unstaged changes in a file.

`git restore --staged filename` – Unstage a file.

`git reset --soft HEAD~1` – Undo latest commit while keeping changes staged.

## Complete Git Workflow

`git clone URL` – Clone repository.

`cd repository-name` – Enter project directory.

`git status` – Check status.

`git add .` – Stage changes.

`git commit -m "Initial commit"` – Commit changes.

`git push origin main` – Upload changes.

`git pull origin main` – Download remote changes.

`git branch feature` – Create branch.

`git checkout feature` – Switch branch.

`git add .` – Stage feature changes.

`git commit -m "Added feature"` – Commit feature.

`git checkout main` – Return to main.

`git merge feature` – Merge feature into main.

`git push origin main` – Upload merged changes.

`git log --oneline` – View commit history.
