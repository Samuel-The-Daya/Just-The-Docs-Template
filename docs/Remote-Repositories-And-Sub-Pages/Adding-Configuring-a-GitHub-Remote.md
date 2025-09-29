---
title: Adding / Configuring a GitHub Remote
parent: Remote Repositories
nav_order: 1
---

<!-- prettier-ignore-start -->

# Adding / Configuring a GitHub Remote 
{: .no_toc }

GitHub is one of many Git version control remote repository services that you can use.

Using GitHub will give you access to remote repositories and allow for you to make changes to your repository from any machine as long as it is all linked to the same repository.

This is also a build up to using GitHub for turning your repository to a collaborative team project.

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