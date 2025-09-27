---
title: Clean
parent: Git Fundamentals
nav_order: 4
---


<!-- prettier-ignore-start -->
# Clean
{: .no_toc }

Clean is a git command that provides a potentially dangerous way to remove untracked files from your working directory.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->


## What is Clean?
Clean offers a much more decisive way of undoing changes. Clean allows you to discard **untracked** files in your working directory. And because it's removing files that have no backups in previous commits, any affected file is permanently gone.

⚠️ ***WARNING***: Using clean can be dangerous. The discarded changes cannot be recovered.



## How to use Clean
If you want to remove a single untracked file from your working directory:
```
git clean <path-or-filename>
```


If you want to remove all untracked files from your working directory:
```
git clean
```