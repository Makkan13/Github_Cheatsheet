# 🧠 Git & GitHub Cheatsheet

### A quick reference for the most useful Git and GitHub commands and concepts.

---

## 📁 Initialize & Clone

```bash
# Start tracking a local folder
git init

# Clone an existing GitHub repository
git clone https://github.com/username/repo.git

# Clone into a specific folder
git clone https://github.com/username/repo.git my-folder
```
---
## 📄 Staging & Committing

```bash
# Check if any files are staged or committed
git status       
     
# Add a specific file
git add filename

# Add all files
git add .

# Commit with a message
git commit -m "Describe your changes"

# Amend the last commit (message or files)  ->(replace the last commit with a new one)
git commit --amend
```
---
## 🔼 Push & Pull

```bash
# Push changes to the main branch
git push origin main

# First push (sets upstream tracking)
git push -u origin main

# Pull the latest changes from the remote
git pull origin main

```
---
## 🔙 Undo & Reset

```bash
# Unstage file (undo git add)
git restore --staged filename

# Discard local changes
git restore filename

# Undo the last commit (keep changes staged)
git reset --soft HEAD~1

# Undo the last commit (keep changes unstaged)
git reset --mixed HEAD~1

# Hard reset to previous state (removes changes!)
git reset --hard HEAD~1

# Revert a specific commit (safely undo)
git revert <commit-hash>
```
---
## 🔍 View History

```bash
# Show commit history
git log

# One-line summary
git log --oneline

# Show history for a specific file
git log filename
```
---
## 🛠️ Configuration
```bash

# Set global username/email
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

# Set config only for current repo
git config user.name "Your Name"
git config user.email "you@example.com"

# Check all settings
git config --list
```
---
## 🌿 Branching
```bash
# List all branches
git branch

# Create a new branch
git branch new-branch

# Switch to a branch
git checkout new-branch

# Create and switch in one step
git checkout -b new-branch

# Delete a branch locally
git branch -d branch-name

# Push a branch to remote
git push origin branch-name

# Track a remote branch
git checkout --track origin/branch-name
```
---
## 🔗 Remote Management
```bash
# Show remotes
git remote -v

# Add a remote repository
git remote add origin https://github.com/username/repo.git

# Change the remote URL
git remote set-url origin https://github.com/newuser/newrepo.git
```
---
## 🚨 Misc & Safety
```bash
# See what's changed
git diff

# See staged changes
git diff --cached    (--staged can be used too same as cached)

# Clean untracked files
git clean -f

# Remove .git folder (uninitialize a repo)
rm -rf .git
```
---
## 🔀 Merging & Rebasing
```bash

# Merge another branch into the current branch
git merge branch-name

# Abort a merge (if conflicts arise and you want to cancel)
git merge --abort

# Rebase your current branch onto another (e.g., sync with main)
git rebase main

# Skip a commit during a rebase
git rebase --skip

# Abort an ongoing rebase
git rebase --abort

#Tip: Use git pull --rebase to avoid unnecessary merge commits:
git pull --rebase origin main
```
---
## 📥Fetching & Comparing
```bash
# Fetch latest changes from remote (no merge)
git fetch origin

# Compare local vs remote branches
git diff main origin/main

# Show remote-tracking branches
git branch -r

# Show all local + remote branches
git branch -a
```
