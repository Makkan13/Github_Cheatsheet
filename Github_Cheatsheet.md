# 🧠 Git & GitHub Cheatsheet

A quick reference for the most useful Git and GitHub commands and concepts.

---

## 📁 Initialize & Clone

```bash
# Start tracking a local folder
git init

# Clone an existing GitHub repository
git clone https://github.com/username/repo.git

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
```
---
## 🔼 Push & Pull

```bash
# Push changes to the main branch
git push origin main

# First push (sets upstream tracking)
git push -u origin main

# Pull updates from remote
git pull origin main

```
---
## 🔙 Undo & Reset

```bash
# Unstage file
git restore --staged filename

# Discard local changes
git restore filename

# Undo last commit (keep files)
git reset --soft HEAD~1

# Hard reset to previous state (removes changes!)
git reset --hard HEAD~1
```
---
## 🔍 View History

```bash
# Show commit history
git log

# One-line summary
git log --oneline
```
---
## 🛠️ Configuration
```bash

# Set global username/email
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

# Check current config
git config --list
```
