---
title: Forking Workflow
parent: The How and Why of Team Git Workflow
nav_order: 4
---

<!-- prettier-ignore-start -->

# Forking Workflow
{: .no_toc }

The **Forking Workflow** is often used for open source projects, in this workflow each developer gets not only their own local repository, but also a server-side copy of the project.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Concepts of the Forking Workflow

These are the base concepts of the Feature Branch Workflow.

- Developers push to their own server-side repositories.

- Changes are shared via pull requests from their personal public repository.

- The project maintainer has the final say on what is merged into the official repository.

_**Note:** This workflow is sometimes called [GitHub Flow](https://docs.github.com/en/get-started/using-github/github-flow)._

## Life Cycle of Forking Workflow

Works like the Feature Branch, except:

1. **Forking:** Each team member creates a fork of the project on the git hosting service.

2. **Cloning:** Team members clone their remote fork to a local repository.

3. **Adding an Upstream:** Team members configure a secondary remote called `upstream` that points to the official repository.

4. **Resolving Conflicts:** Remote commits from `upstream` can be pulled into the local feature branch, with merge conflicts resolved as required.

5. **Pushing to Remote:** Local feature branches are pushed to the forked remote.

6. **Requesting a Remote Merge:** Pull request are initiated to request merges from the remote fork to the official upstream repository.

## Source

[https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531991/View](https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531991/View).