---
title: Reset
parent: Git Fundamentals
nav_order: 2
---

<!-- prettier-ignore-start -->
# Reset
{: .no_toc }

Reset is a git command that provides a dangerous and potentially destructive way to undo commits in a git repository.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->


## What is Reset?
⚠️ ***WARNING***: Using reset is dangerous. It rewrites your repository's history by changing the HEAD pointer. Commits after the reset point are not "lost", but they can become difficult to recover.

A git reset comes in three flavors, each affecting the repository differently:
- Hard Reset (Dangerous): Resets the HEAD pointer, staging area, and your working directory to match a specific commit. All uncommitted changes are lost when they are reset to the specified commit.

- Mixed Reset (Weirder): Resets the HEAD pointer and the staging area, but keeps the changes in your working directory. The HEAD and your working directory may differ if you had uncommitted changes.

- Soft Reset (Weird): Resets the HEAD pointer, but keeps the changes in the staging area and working directory. The HEAD and your working directory may differ if you had uncommitted changes.


## How to use Reset

To do a Hard Reset: 
```
git reset --hard [commit id]
```


To do a Soft Reset: 
```
git reset --soft [commit id]
```


To do a Mixed Reset: 
```
git reset --mixed [commit id]
```

To look at work in an old commit, before returning to where you were:
```
git reset --hard [B] (reset to commit B)

git reset --hard [D] (reset back to commit D)
```