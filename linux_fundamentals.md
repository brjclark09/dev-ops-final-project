---
title: "Linux Fundamentals"
author: "Brandon Clark"
description: "A summary of what I've learned this semester for the topic of linux."
published: "2024-2-14"
---
# Linux Fundamentals
## Commands
Installing git on linux based systems:
- `sudo dnf install git` for RedHat variants
- `sudo apt install git` for Ubuntu variants

Changing target directory:
- `cd [FILEPATH]`
- `cd ..` moves up a folder

Making a folder:
- `mkdir "name"`
- `mkdir -p "name"` for adding multiple folders

Create a file:
- `touch [FILENAME]` with file extension

Removing a file:
- `rm [FILENAME]`

Removing a folder:
- `rmdir [FOLDERNAME]`

Showing current directory path:
- `pwd`

Lists the current folder's files:
- `ls`

Move or rename files:
- `mv`

Copy files:
- `cp`

Add a user:
- `sudo adduser [USERNAME] -c "name"`

Add a password to the user:
- `sudo passwd [USERNAME] [PASSWORD]`

Create a permissions group:
- `sudo groupadd [GROUPNAME]`

Add a user to a permissions group:
- `sudo usermod [USERNAME] -aG [GROUPNAME]`

Changing the permissions of a file or folder:
*Permission levels are user (u), group (g), and other (o).
- `sudo chmod g=rx [FOLDER OR FILENAME]`

Changing the user ownership of a file or directory:
- `sudo chown [CURRENTOWNER] [FUTUREOWNER]`

Changing the group ownership of a file or directory:
- `sudo chgrp [CURRENTOWNER] [FUTUREOWNER]`

See permissions:
- `ls -la` permissions are read, write, execute (rwx) for each level's access

Update the list of packages / software:
- `sudo dnf update`
- `sudo dnf upgrade`

Install a package / software:
- `sudo apt install nginx`

Starting a package / software:
- `sudo systemctl enable nginx`
- `sudo systemctl start nginx`
- `sudo systemctl status nginx`