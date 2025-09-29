---
title: Resolving Merge Conflicts
nav_order: 6
---


<!-- prettier-ignore-start -->
# Resolving Merge Conflicts
{: .no_toc }

Merge conflicts occur when Git can't automatically merge two branches. This section includes information on how to resolve these conflicts.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## How Git Marks Conflicted Files

Git uses special markers to indicate the start and end of the conflicted area:

- ```<<<<<<< HEAD``` : shows the start of the changes in the current branch.
- ```=======``` : separator between the changes in the current and the other branch.
- ```>>>>>>> branch-name``` : shows the end of the changes in the other branch.

The end result looks something like this:

```
<<<<<<< HEAD

Value = 5

=======

Value = 10

>>>>>>> BRANCH
```


## Resolving Merge Conflicts
To resolve a merge conflict:

1. Edit the file to fix the conflicting changes. *Be sure to remove the conflict markers.*
2. Add the file to the staging area with ```git add``` .
3. Commit the fix with ```git commit``` .