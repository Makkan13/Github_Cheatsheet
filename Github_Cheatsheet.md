# 🧠 Git & GitHub Cheatsheet

A quick reference for the most useful Git and GitHub commands and concepts.

---

## 📁 Initialize & Clone

```bash
# Start tracking a local folder
git init

# Clone an existing GitHub repository
git clone https://github.com/username/repo.git

## 📄 Staging & Committing

``bash
git status

# Add a specific file
git add filename

# Add all files
git add .

# Commit with a message
git commit -m "Describe your changes"

## 🔼 Push & Pull

``bash
# Push changes to the main branch
git push origin main

# First push (sets upstream tracking)
git push -u origin main

# Pull updates from remote
git pull origin main
