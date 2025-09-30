---
title: Checkout
parent: Git Fundamentals
nav_order: 1
---

<!-- prettier-ignore-start -->
# Checkout
{: .no_toc }

Checkout is a git command that provides a simple, yet slightly dangerous way to undo uncommitted work in a git repository.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->


## What is Checkout?
Checkout is the simplest way to privately undo work in a git repository. It allows you to discard any **unstaged** and **uncommitted** changes to **tracked** files in a local git repository.

⚠️ ***WARNING***: Using checkout can be slightly dangerous. The discarded changes cannot be recovered.


## How to use Checkout
If you want to revert changes to a single unstaged file to the most recent commit:
```
git checkout <path-or-filename>
```


If you want to revert changes to all unstaged files and folders to the most recent commit:
```
git checkout .
```


## Sources
- [Class Notes on ```git checkout```](https://stungeye.github.io/Software-Development-And-Documentation-1/02-git-version-control-next-steps/index.html#4)