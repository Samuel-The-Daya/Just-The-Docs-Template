---
title: Overview of Git Workflows
parent: The How and Why of Team Git Workflow
nav_order: 1
---

<!-- prettier-ignore-start -->

# Overview of Git Workflows
{: .no_toc }

Working with a team, each team member must be knowledgeable on how the Git Workflow works.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Collaborative Coding with Git and GitHub

With Git and GitHub, multiple developers can work on the same project without stepping on each other's toes.

Key concepts include:

- Forking: Creating a personal copy of another user's repository.
- Cloning: Downloading a repository to your local machine.
- Committing: Saving changes to the local repository.
- Pushing: Sending committed changes to a remote repository.
- Pull Request: Proposing changes to a repository that can be reviewed and potentially merged.

## Overview of Git Workflows

Git workflows are methods or procedures that dictate how developers interact with the Git system to achieve effective team collaboration.

There are several popular workflows used by teams:

- Centralized Workflow

- Feature Branch Workflow

- Forking Workflow

## Pull Requests

- Mechanism to propose changes to a repo and facilitate discussion about them.

- The project maintainers, and potentially other contributors, can:

    - Review the changes

    - Comment on them

    - Suggest modifications

    - Approve or close the request

- Pull requests are not part of git proper.

- They are facilitated by git hosting solutions like GitHub.

## Creating Pull Requests

Pull requests are opened via the GitHub.com page for the repository.

Git GUIs (like Visual Studio) will often provide you with a link to create a request after pushing changes to a remote branch.

## Pull Request Merge Conflicts

You will be prevented from creating a pull request if your branch can't be merged.

To resolve the conflict:

- Locally checkout the `main` branch.

- Pull the latest changes into `main` from the remote.

- Checkout your branch. (The one you wanted to merge.)

- Merge `main` into your branch.

- Resolve the conflicts using your editor or merge tool.

- Commit your changes to your branch.

- Push your branch to the remote.

- Attempt to create the pull request again.

## Source

[https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531991/View](https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531991/View).