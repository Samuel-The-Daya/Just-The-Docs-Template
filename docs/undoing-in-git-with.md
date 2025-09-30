---
title: Undoing in Git with
has_children: true
nav_order: 4
---



# Undoing in Git with...

One of the biggest benefits of Git and version control in general is the ability to *"hit the undo button"* as it were, returning aspects of your working directory to a previous snapshot you've taken.

This Module will cover four different ways you can do that using Git, how those methods differ and when to use each one.


## Objectives

Upon completion of this module, you should be able to:

- Tell the difference between ```git checkout```, ```git reset```, ```git revert```, and ```git clean```.
- Use ```git checkout``` to "revert" work done on one or more unstaged files to the most recently committed version.
- Tell the difference between the three types of ```git reset```.
- Use ```git reset``` to return to a previous commit to check an older version of a file, then ```git reset``` again to return to the most recent commit you made.
- Use ```git revert``` to publicly undo one or more commits.
- Use ```git clean``` to remove one or more untracked files from your working directory.
- Know when to use any of the commands listed above.

## Sources

- [Class Notes](https://stungeye.github.io/Software-Development-And-Documentation-1/02-git-version-control-next-steps/index.html#3) 
                ([```git checkout```](https://stungeye.github.io/Software-Development-And-Documentation-1/02-git-version-control-next-steps/index.html#4), 
                 [```git reset```](https://stungeye.github.io/Software-Development-And-Documentation-1/02-git-version-control-next-steps/index.html#6),
                 [```git revert```](https://stungeye.github.io/Software-Development-And-Documentation-1/02-git-version-control-next-steps/index.html#11))
- [An explanation of ```git reset``` including Mixed Resets](https://practicalseries.com/1002-vcs/02-05-concept.html#js--020505)
- [Documentation for ```git clean```](https://git-scm.com/docs/git-clean)