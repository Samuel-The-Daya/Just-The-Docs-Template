---
title: Centralized Workflow
parent: The How and Why of Team Git Workflow
nav_order: 2
---

<!-- prettier-ignore-start -->

# Centralized Workflow
{: .no_toc }

The **Centralized Workflow** is about working on a single branch.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Concepts of the Centralized Workflow

These are the base concepts of the Centralized Workflow.

- Simple and similar to Subversion-style workflows.
- Not as powerful or flexible as other workflows.
- Suitable for small teams and projects.
- Merging can be problematic.

## Life Cycle of Centralized Workflow

1. Initialization: One team member creates the repository with an online remote.

2. **Cloning:** Each team member creates a local copy by "cloning" the remote.

3. **Working Locally:** Developers work on the project, committing to their local repository.

4. **Resolving Conflicts:** When a developer is ready to share their changes, they must pull outstanding changes from the remote, and resolve merge conflicts as required.

5. **Pushing to Remote:** The developer can now push their changes to the central repository.

6. **Synchronizing Team:** Others can now pull from the central repository to locally incorporate the latest changes.

## Source

[https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531991/View](https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531991/View).