---
title: Pushing and Pulling
parent: Remote Repositories
nav_order: 2
---

<!-- prettier-ignore-start -->

# Pushing and Pulling
{: .no_toc }

Pushing and Pulling are the two main commands to using a remote repository.

This module will teach you the GitHub workflow and also the best practices of pushing and pulling.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## GitHub Workflow

If you want to make a copy of a GitHub repository to your local machine, you can **clone** it:

```
git clone git@github.com:<INSERT-YOUR-GITHUB-USERNAME>/<INSERT-YOUR-REPOSITORY-NAME>.git
```

Once you have your local and remote repository set up, you can **push** and **pull** changes.

## Pushing

When you want to send your commits of the local repository to GitHub:

```
git push origin <INSERT-YOUR-BRANCH-NAME>
```

With this command your local commits on the repository will be sent to the GitHub repository.

This links all your changes to the remote repository, but not your future changes, you must push whenever you wish to send a change.

Think of it as making documents that you then fax over to your office.

## Pulling

When you want to grab the latest commits from your remote repository on GitHub:

```
git pull origin <INSERT-YOUR-BRANCH-NAME>
```

If your repository is not updated to the current state of the remote repository, pulling will update your local repository.

It is best practice to pull before pushing to avoid merge conflicts.

**Important:** If you made any commits on your local repository before pulling, you may run into **merge conflicts** that you have to resolve.

## When To Push and Pull

There are multiple philosophies that people follow when pushing and pulling.

Common times people push:

- After every commit.

- If in a branch with a team, alternating with team members.

- Before closing the repository for the day.

Common times people pull:

- Before beginning to work on the repository for the day.

- If in a branch with a team, Whenever a push is made from another team member.

It is best to always pull before starting work and push everytime finishing work.

## Sources & Additional Links

[Class Notes](https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531990/View).

[Pushing Commits to a remote repository](https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository).

[Getting changes from a remote repository](https://docs.github.com/en/get-started/using-git/getting-changes-from-a-remote-repository).