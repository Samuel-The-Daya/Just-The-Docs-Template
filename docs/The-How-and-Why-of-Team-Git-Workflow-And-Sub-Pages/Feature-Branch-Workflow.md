---
title: Feature Branch Workflow
parent: The How and Why of Team Git Workflow
nav_order: 3
---

<!-- prettier-ignore-start -->

# Feature Branch Workflow
{: .no_toc }

The **Feature Branch Workflow** is about working feature development or bug fixes on dedicated branches for each feature / fix.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Concepts of the Feature Branch Workflow

These are the base concepts of the Feature Branch Workflow.

- Isolates new development from the main branch.

- Makes it easy to discard experimental changes.

- Facilitates code review via pull requests.

_**Note:** This workflow is sometimes called [GitHub Flow](https://docs.github.com/en/get-started/using-github/github-flow)._

## Life Cycle of Feature Branch Workflow

1. **Branching:** New features or fixes are developed locally in a short-lived branch.

2. **Resolving Conflicts:** Remote commits by other developers can be pulled into the local feature branch, with merge conflicts resolved as required.

3. **Pushing to Remote:** Completed and resolved branches are then pushed.

4. **Requesting a Remote Merge:** A pull request is next initiated on the git hosting service (example; GitHub).

5. **Reviewing:** One or more team members review the pull request before merging it into the main remote branch.

_**Note:** Pull requests can be sent back unmerged if rework is deamed necessary._

## Source

[https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531991/View](https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531991/View).