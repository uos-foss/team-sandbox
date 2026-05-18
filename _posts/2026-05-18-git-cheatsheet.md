---
layout: post
title: Git Cheat Sheet
subtitle: Cheat sheet for gits
author: Bill Smith
---

Here is a clean, survival Git cheat sheet organized by what you are actually trying to accomplish. It covers everything from starting a fresh project to saving your work and fixing mistakes.

---

## 🛠️ The Absolute Basics (Starting out)

Use these commands when you are setting up your project for the first time or grabbing it from GitHub.

|**Command**|**What it does**|
|---|---|
|`git init`|Initializes a brand new, empty local Git repository in your current folder.|
|`git clone <url>`|Downloads an existing repository from GitHub to your computer.|
|`git status`|The most useful command. Shows you which files have been changed, added, or deleted.|

---

## 💾 Saving Your Work (The Daily Loop)

Think of this as the "Save Game" process. You track changes, bundle them up, and label them.

Bash

```
# Step 1: Add a specific file to the staging area (preparing to save)
git add filename.txt

# Or, add ALL changed files at once:
git add .

# Step 2: Permanently save your staged changes with a descriptive note
git commit -m "Fix: Resolved login button alignment"
```

---

## 🌳 Branching (Working Safely)

Branches let you work on new features or text edits without messing up the working (`main`) code.

Bash

```
# List all local branches (the one with the * is your current branch)
git branch

# Create a brand new branch and immediately switch to it
git checkout -b feature/new-blog-post

# Switch back to an existing branch (like main)
git checkout main

# Delete a branch locally (do this after it's successfully merged)
git branch -d feature/old-branch
```

---

## 🌐 Syncing with GitHub (Sharing)

Use these to move code between your local computer and the cloud (GitHub).

Bash

```
# Download the absolute latest changes from GitHub into your current branch
git pull origin main

# Upload your local commits to your branch on GitHub for the first time
git push -u origin feature/new-blog-post

# Upload your local commits if the branch already exists on GitHub
git push origin
```

---

## 🚨 Emergency / Fixing Mistakes

Did something go wrong? Don't panic. Use these to hit the undo button.

Bash

```
# Undo 'git add' — takes a file out of the staging area, but keeps your edits
git reset filename.txt

# Discard ALL local changes in your working directory since your last commit
# (WARNING: This completely wipes out uncommitted work!)
git reset --hard HEAD

# Modify your very last commit message (great for fixing typos in your note)
git commit --amening -m "New and correct commit message"

# Show a history of all previous commits in this branch
git log --oneline
```