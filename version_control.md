---
title: "Version Control"
author: "Brandon Clark"
description: "A summary of what I've learned this semester for the topic of version control."
published: "2024-2-14"
---
# Version Control
## Commands
Installing git on linux based systems:
- `sudo dnf install git` for RedHat variants
- `sudo apt install git` for Ubuntu variants

Initalize a repository:
- `git init`

Linking a repository:
- `git remote add origin [LINK]`

Clone a repository:
- `git clone [LINK]`

Adding files to a commit:
- `git add .` for adding all files
- `git add [FILENAME]` for adding a specific file

Committing files:
- `git commit -m "message"`

Pushing files:
- `git push origin master` for pushing files to the master branch

Pulling files:
- `git pull origin master` for pulling files from the master branch

Viewing the log:
- `git log`

Adding a new branch:
- `git branch [BRANCHNAME]`

Switching to a branch:
- `git switch [BRANCHNAME]`