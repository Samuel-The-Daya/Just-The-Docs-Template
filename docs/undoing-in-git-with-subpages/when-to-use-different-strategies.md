---
title: When to Use Different Strategies
parent: Git Fundamentals
nav_order: 5
---

<!-- prettier-ignore-start -->
# When to Use Different Strategies
{: .no_toc }

There are a number of ways to undo work in a repository, so here we'll go through which methods to use for specific scenarios.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->


## When to use Checkout
Use ```git checkout``` if: 
- You want to undo changes that haven't yet been committed. (Dirty files.)
- You want to revert to the most recently committed version of a file or files.


## When to use Reset

Use ```git reset``` if: 
- You want to undo one or more commits in your local repository.
- You want to take a look at an older commit without making changes, then reset back to the main HEAD.
- You want to make a branch of an older commit. (remember to reset the origin branch back to the main HEAD afterwards)


## When to use Revert
Use ```git revert``` if:
- You want to undo a commit that has been shared with others. This allows you to keep a record of any mistakes made.
- You have committed changes, but you want to play it safe and not risk any damage to your repository.


## When to use Clean
Use ```git clean``` when you want to remove untracked files from your working directory.