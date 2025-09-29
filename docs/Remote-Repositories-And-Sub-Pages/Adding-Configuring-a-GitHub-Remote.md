---
title: Adding / Configuring a GitHub Remote
parent: Remote Repositories
nav_order: 1
---

<!-- prettier-ignore-start -->

# Adding / Configuring a GitHub Remote 
{: .no_toc }

Working with multiple people or making different types of changes can lead to chaos if it is unorganized.

**Branches** allows for creating multiple changes on the repository in a separate "version without affecting the project unless needed to be.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Introduction to GitHub

There are numerous ways with setting up a remote repository using Git. A very common option is to use GitHub.

GitHub is a hosting platform for Git repositories owned by Microsoft.

It provides a web-based interface to interact with your repositories and adds social and collaboration features.

## Remote Repository / GitHub Terminology

**Push**: Send commits made on a local repository to the remote repository. Send changes to the remote repository.

**Pull**: Fetch and merge changes from a repository into the current branch. Used to keep local repositories up to date with remote repository.

**Clone**: May a full copy of a repository at its current state. Commonly use to make a copy of a remote repository to to a local repository.

## Adding Repositories to GitHub

Before linking a local repository to GitHub, make sure that you have a GitHub account set up.

To save a local git repository to your GitHub account, create a new repository by way of the "+" button in the top right corner of the GitHUb website.

**IMPORTANT:** Be sure not to initialize with a README or with any other files

## Linking Your Local Repository to GitHub

To link a local repository to GitHub, you take your repository name, for this example its `My-Repository`. Make sure it is an initialized Git repository.

From the command line (within the project folder) add GitHub as a remote:

```

git remote add origin git@github.com:<INSERT-YOUR-GITHUB-USERNAME>/My-Repository.git

```

_Reminder that `<INSERT-YOUR-GITHUB-USERNAME>` should be replaced with your GitHub username._

Check if the remote has been added to a repository:

```

git remote -v

```

## GitHub Worflow

If you want to make a copy of a GitHub repository to your local machine, you can **clone** it:

```

git clone git@github.com:<INSERT-YOUR-GITHUB-USERNAME>/<INSERT-YOUR-REPOSITORY-NAME>.git

```

When you want to send your commits of the local repository to GitHub:

```

git push origin <INSERT-YOUR-BRANCH-NAME>

```

When you want to grab the latest commits from your remote repository on GitHub:

```

git pull origin <INSERT-YOUR-BRANCH-NAME>

```