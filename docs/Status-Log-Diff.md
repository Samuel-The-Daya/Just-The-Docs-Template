---
title: History
parent: Git-Fundamentals 
nav_order: 4
---

<!-- prettier-ignore-start -->
# Status, Log and Diff
{: .no_toc }

Status, Log and Diff are all git commands that help the user manage their projects. Status allows the user to check the status of their repo. Log allows the user to show the history of commits. Finally Diff allows users to compare files between commits. 

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->
## Checking Your Repo's Status
To check the status of the repo for changes or additions:

``git status``

Open Windows Explorer:

``explorer.exe .``

And then create a ``readme.md`` file.

## Log
### Git Commits and the Git Log
Commits can be reviewed by using:
``git log``
Each entry in the log shows:
- The commit hash.
- Who made the commit.
- When it was made.
- The commit message.

The 40 character hex numbers shown at the start of each entry are the SHA1 hashes
that uniquely identify each commit.

![a screen shot of an example of the commit message: Commit f2c87c8e (this hash is very long, as long as you have the first 8 digits you will be able to track it again) Author: Kyle Geske (userEmail) Date: Wed Sept 19 13:46:09 2018, (Commit message)"Added find_by and update_all to appropriate demo files"](image.png)

## Diff 
### What's the Difference
To compare the differences between the current files and the last commit:
``git diff``

We can diff specific files:
``git diff secret_plans.txt``

Or specific folders (and their sub-folders):
``git diff ./textfiles/plans``