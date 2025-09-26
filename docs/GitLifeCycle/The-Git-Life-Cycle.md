---
layout: default
title: The Git Life Cycle
nav_order: 2
---

# The Git Life Cycle 

The Git Life Cycle is the different stages the files and directory goes through when working with Git.


As you work with Git, it is best to be updated on the terminology and be knowledgable on the different states the directory and files goes through.

## Directory

There are three states that the directory goes through as you use Git Version Control.

- Working Directory

- Staging Area

- Git Directory

### Working Directory

In a local directory, as you make it a git repository by using the `git init` command, you let git become aware of your files and keeps track of your **Working Directory**.

```
git init
```

The working directory is the current state of your repository's files on disk.

As you add, delete or make changes on your files and other data types, the working directory saves all that data.

### Staging Area

Now Git can save a **version** of your working directory or a specific file to the **Staging Area**.

If you are working on a full project and need to save a lot of files at once, you can save the entire working directory by using `git add .` or a specific file with `git add <FILENAME>`.

There are several reasons to save a specific file, but a common reason is there are other files that are modified and you do not want to Git to stage them.

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

Committing saves the metadata of the files in the staging area at that **current version**.

Basically saves a snapshot of your repository at that time.

You are able to include a commit messsage as you commit your files to explain / describe the status of the repository during the time you made the commit.

```

// Commit staged files with a commit message. 

git commit -m <INSERT-COMMIT-MESSAGE-HERE>

```

## Sources
[https://www.geeksforgeeks.org/git/git-life-cycle](https://www.geeksforgeeks.org/git/git-life-cycle).