---
title: Stashing
nav_order: 7
---


<!-- prettier-ignore-start -->
# Stashing
{: .no_toc }

```git stash``` allows you to put aside changes that you don't want to commit immediately. 

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Stashing Changes: The Magic Toy Box

Think of stashing like a magic toy box. 

It allows a kid to instantly clean their room, and when they want to play again, all toys are returned to their former positions.

It allows you to temporarily store the state of your working directory, then restore that state when you need it.

## The Stash Stack

Think of ```git stash``` as creating a stack of saved changes.

You can stash multiple sets of changes and Git will store them in a LIFO (Last in, First Out) stack.

## When to Stash

- You want to switch branches, but you're in the middle of something and don't want to commit yet.
- You need to pull changes, but you have uncommitted work.

## Stashing in Action
```
git stash
```
This command stashes your changes, leaving you with a clean working directory.

**Remember, it's only a temporary storage. Don't forget about your stashed changes!**
## Restoring Stashed Changes
To restore stashed changes, use:

- ```git stash pop``` - Re-applies the changes and removes them from the stash.
- ```git stash apply``` - Re-applies the changes but keeps them in the stash.

## Other Helpful Stash Commands
```git stash list``` : Review all your stashes before deciding to apply or drop them.

```git stash drop``` : Removes the most recent stash from the stack without applying it.

```git stash branch <branchname>``` : Creates a new branch based on the popped stash.

```git stash clear``` : This command removes all your stashes.

```git stash pop 'stash@{n}'``` : Pop a specific stash seen in ```git stash list``` .

## Sources
- [Class Notes](https://stungeye.github.io/Software-Development-And-Documentation-1/02-git-version-control-next-steps/index.html#27)