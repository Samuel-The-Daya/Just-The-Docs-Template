---
layout: default
title: Creating, Using, and Merging Branches
nav_order: 5
---

<!-- prettier-ignore-start -->

# Creating, Using, and Merging Branches 
{: .no_toc }

Working with multiple people or making different types of changes can lead to chaos if it is unorganized.

**Branches** allows for creating multiple changes on the repository in a separate "version without affecting the project unless needed to be.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Introducing Branches

In Git, branches are like alternate timelines in a sci-fi movie.

They allow you to work on different features or fixes without affecting the main project
timeline until you choose to merge the timelines back together.

## Creating Branches

Creating a new branch:

```

git branch <branch-name>

```

This will create a new branch in your repository, creating a seperate "timeline" of your project.

Switching to a branch:

```

git checkout <branch-name>

```

Switching branches will move you to the branch that you want to work in. Making commits in that branch keeps all your commits to that branch and nowhere else.

Create and switch in a single command:

```

git checkout -b <branch-name>

```

The fastest way to create and switch branches.

## Merging Branches

Branching allows for isolated development, and merging brings those developments
back into the main timeline.

Let's say we've been working and committing to an experimental branch and we
want to merge those commits back into main:

```

git checkout main
git merge experimental

```

Merging will bring all the commits made in the separate branch back to main and update the state of the project like it was in the branch, while also linking it with any additional commtis made in main.

## Merge Conflicts

Merge conflicts occur when Git can't automatically merge two branches.

When a merge conflict happens, Git will alert you in the terminal and mark the areas of
conflict in the file.

## Git's Markup of Conflicted Files

Git uses special markers to indicate the start and end of the conflicted area:

`<<<<<<< HEAD` shows the start of the changes in the current branch.

`=======` separator between the changes in the current and the other branch.

`>>>>>>> branch-name` shows the end of the changes in the other branch.

## Resolving Merge Conflicts

To resolve a merge conflict:
1. Edit the file to fix the conflicting changes. Be sure to remove the conflict markers.
2. Add the file to the staging area with `git add`.
3. Commit the fix with `git commit`.

## Sources
[https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531990/View](https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531990/View).