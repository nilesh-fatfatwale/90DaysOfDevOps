# 🚀 Day 14 - Git & GitHub

## ✅ Topics Covered

### 🔧 What is Git?
- Git stands for **Global Information Tracker**
- Created by **Linus Torvalds**
- A distributed version control system (VCS)
- Helps track changes, manage code, collaborate with teams

### 🔗 Types of Version Control Systems
- GitHub
- GitLab
- Bitbucket

### 📁 VCS vs File System
| File System | VCS |
|-------------|-----|
| Tracks latest version only | Tracks full history |
| Manual backups | Automated versioning |
| Difficult to collaborate | Easy to collaborate & merge |


git init                # Initialize a git repository
git add <file>          # Add file to staging
git commit -m "msg"     # Commit staged files
git rm --cached <file>  # Remove from staging
git restore <file>      # Restore file to last commit
git status              # See current state

---

## ⚙️ Git Configuration & Setup

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```
## Git Commands Practiced
```bash
git init                # Initialize a git repository
git add <file>          # Add file to staging
git commit -m "msg"     # Commit staged files
git rm --cached <file>  # Remove from staging
git restore <file>      # Restore file to last commit
git status              # See current state

```
🌿 Branching
Create & switch branches:

```bash
git branch               # List branches
git checkout -b dev      # Create & switch to new branch
git switch dev           # Switch branch (alternative)

```
- Why Branching?

Parallel development

Safer code experimentation

Feature isolation

- main vs master

Older Git used master as the default branch

Now replaced with main to support inclusive naming

## Merging Branches
```bash
git checkout main
git merge dev

```
##🔒 Authentication
SSH Key Setup

Personal Access Token (PAT)

##🚫 .gitignore
Used to ignore files from being tracked (e.g., .env, node_modules/, *.log)

##🌱 Branching Strategies
Feature Branch

Git Flow

Trunk-Based Development

##🔗 Jira + GitHub Integration
Automate workflows

Link commits to issues

Track progress effectively

##⏪ Reset & Revert
```bash

git reset --soft <commit>
git reset --mixed <commit>
git reset --hard <commit>
git revert <commit>

```
##🧳 Stashing
```bash
git stash            # Save uncommitted changes
git stash pop        # Retrieve them later

```
##🍒 Cherry Pick
```bash
git cherry-pick <commit-hash>

```
[Previous Day →](../Day-13/README.md)                                                                                    [Next Day →](../Day-15/README.md) 
