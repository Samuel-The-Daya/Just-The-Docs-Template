---
layout: default
title: The Git Life Cycle
nav_order: 2
---

<!-- prettier-ignore-start -->

# The Git Life Cycle 
{: .no_toc }

Git tracks and saves the metadata of files in its directory as you use Git for version control. 

The Git Life Cycle is the different stages that files goes through within the directory.


## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Directory

There are three states that the directory goes through as you use Git Version Control.

- Working Directory

- Staging Area

- Git Directory

### Working Directory

In a local directory/folder, awhen you use the `git init` command (creating a repository), you let git become aware of your files and keeps track of your **Working Directory**.

```
git init
```

The working directory is the current state of your repository's files on disk.

As you add, delete or make changes on your files and other data types, the working directory saves all that data.

### Staging Area

Now Git can add a current version of your working directory or a specific file to the **Staging Area**.

If you are working on a full project and need to save a lot of files at once, you can save the entire working directory by using `git add .` or a specific file with `git add <FILENAME>`.

```
// To add the working directory to the staging area

git add .

// To add a specific file

git add <FILENAME>

// To add a file in a specific folder

git add ..\<FILENAME>
```

### Git Directory

Once files are staged, they are ready to be **committed** to the **Git Directory**.

Committing saves the metadata of the files in the staging area at that **current version** and saves them in the '.git' folder. Basically saves a snapshot of your repository at that time.

You are able to include a commit messsage as you commit your files to explain / describe the status of the repository during the time you made the commit.

```
// Commit staged files with a commit message.

git commit -m <INSERT-COMMIT-MESSAGE-HERE>
```

## Files

There are four states that files can go through during the Git Life Cycle:

- Untracked

- Staged

- Unmodified

- Modified

![The Git Life Cycle](lifecycle.png)

### Untracked

When a file is initialized, it is first **untracked**.

### Unmodified

Once the files are committed, the metadata is saved to Git and since that version of the file is saved, it is now **unmodified**.

Once you edit the file and make changes, it becomes **modified**.

### Modified

When a change is made to an unmodified file, it is considered modified. Once a file is modified, it needs to be **staged** once more before it can be committed.

### Staged

When it is staged, the file is tracked by Git and ready to be committed.

A file that is **untracked** or **modified** cannot be committed to a repository. Once said file is added to the staging area, it is considered **staged**.

## Sources & Additional Links
[Picture Source](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository).

[Git Life Cycle](https://www.geeksforgeeks.org/git/git-life-cycle).

[Stages in Git Life Cycle](https://www.toolsqa.com/git/git-life-cycle).

[Git Life Cycle Diagram](https://www.tutorialspoint.com/git/git_life_cycle.htm).