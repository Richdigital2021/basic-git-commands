# Basic Git Commands

A comprehensive guide to basic Git commands, their descriptions, example usage, and scenarios for when to use them.

---

## **Repository Setup**

| Command | Description | Example Usage | Scenario |
|---------|-------------|---------------|----------|
| `git init` | Initializes a new Git repository. | `git init` | When starting a new project and setting up version control. |
| `git clone <repo_url>` | Clones a repository from a remote source. | `git clone https://github.com/user/repo.git` | When working on an existing project from a remote repository. |

---

## **Tracking Changes**

| Command | Description | Example Usage | Scenario |
|---------|-------------|---------------|----------|
| `git status` | Shows the working directory status. | `git status` | When checking which files have been modified or staged before committing. |
| `git add <file>` | Stages a specific file for commit. | `git add index.html` | When preparing specific files for a commit. |
| `git add .` | Stages all modified files for commit. | `git add .` | When committing all changes made in the working directory. |
| `git commit -m "<message>"` | Commits staged changes. | `git commit -m "Initial commit"` | After adding files to the staging area, to save the changes. |

---

## **Branching & Merging**

| Command | Description | Example Usage | Scenario |
|---------|-------------|---------------|----------|
| `git branch` | Lists all local branches. | `git branch` | When checking available branches in a repository. |
| `git branch <branch_name>` | Creates a new branch. | `git branch feature-branch` | When starting work on a new feature. |
| `git checkout <branch_name>` | Switches to another branch. | `git checkout feature-branch` | When working on a different branch or reviewing code. |
| `git checkout -b <branch_name>` | Creates and switches to a new branch. | `git checkout -b hotfix` | When quickly creating and switching to a new branch for a fix. |
| `git merge <branch_name>` | Merges a branch into the current branch. | `git merge feature-branch` | When integrating changes from a feature branch into main. |
| `git branch -d <branch_name>` | Deletes a branch locally. | `git branch -d old-branch` | After merging, when cleaning up unnecessary branches. |

---

## **Remote Repository Management**

| Command | Description | Example Usage | Scenario |
|---------|-------------|---------------|----------|
| `git remote -v` | Lists remote repositories. | `git remote -v` | When verifying which remote repositories are linked. |
| `git remote add <name> <url>` | Adds a new remote repository. | `git remote add origin https://github.com/user/repo.git` | When connecting a local repository to a remote service like GitHub. |
| `git push <remote> <branch>` | Pushes commits to a remote repository. | `git push origin main` | After committing, to update the remote repository with changes. |
| `git pull <remote> <branch>` | Fetches and merges remote changes. | `git pull origin main` | When updating the local repository with the latest remote changes. |
| `git fetch <remote>` | Downloads remote changes without merging. | `git fetch origin` | When checking for updates before merging changes. |

---

## **Undoing Changes**

| Command | Description | Example Usage | Scenario |
|---------|-------------|---------------|----------|
| `git reset <file>` | Unstages a file. | `git reset index.html` | When removing a file from the staging area before committing. |
| `git reset --hard` | Resets all changes permanently. | `git reset --hard` | When discarding all local changes and resetting to the last commit. |
| `git revert <commit>` | Creates a new commit that undoes a previous commit. | `git revert abc123` | When rolling back a commit without losing history. |
| `git checkout -- <file>` | Discards local changes to a file. | `git checkout -- index.html` | When restoring a file to its last committed state. |

---

## **Stashing Changes**

| Command | Description | Example Usage | Scenario |
|---------|-------------|---------------|----------|
| `git stash` | Saves uncommitted changes. | `git stash` | When switching branches without committing changes. |
| `git stash apply` | Restores the most recent stash. | `git stash apply` | When applying previously saved changes. |
| `git stash pop` | Applies and removes the last stash. | `git stash pop` | When restoring changes while removing them from the stash. |

---

## **Tagging**

| Command | Description | Example Usage | Scenario |
|---------|-------------|---------------|----------|
| `git tag <tag_name>` | Creates a new tag. | `git tag v1.0` | When marking a specific commit as a release version. |
| `git push --tags` | Pushes all tags to remote. | `git push --tags` | When publishing version tags to a remote repository. |

---

## **Logging & History**

| Command | Description | Example Usage | Scenario |
|---------|-------------|---------------|----------|
| `git log` | Shows commit history. | `git log` | When reviewing past commits and messages. |
| `git log --oneline` | Shows a condensed commit history. | `git log --oneline` | When quickly viewing the commit history. |
| `git blame <file>` | Shows line-by-line history of a file. | `git blame index.html` | When tracking changes to a specific file. |

---

## **Configuration & Miscellaneous**

| Command | Description | Example Usage | Scenario |
|---------|-------------|---------------|----------|
| `git config --global user.name "<name>"` | Sets the global username. | `git config --global user.name "John Doe"` | When configuring Git for the first time. |
| `git config --global user.email "<email>"` | Sets the global email. | `git config --global user.email "john@example.com"` | When setting up Git identity for commits. |
| `git config --list` | Displays Git configuration settings. | `git config --list` | When verifying Git configurations. |
| `git help <command>` | Displays help information for a command. | `git help commit` | When needing documentation on a specific command. |
