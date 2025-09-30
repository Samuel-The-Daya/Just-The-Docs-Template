---
title: History
parent: Git-Fundamentals 
nav_order: 3
---
#Staging and Committing 
## Staging Files Before we Commit
As we make changes to our code we **commit** the changes to our git repo.
Before we can **commit** we must **add** new or changed files to a staging area.

**Let's stage our new readme.md file:**
``git add readme.md``
We could also use a period to stage all new or modified files:
``git add .``

Wilcards and sub-folders work too:
``git add docs/textfiles/*.txt``

## Committing Staged Files
We **commit** our staged changes with a commit message.
For complex changes, we can include a short title, followed by a long explaination:

``` 
git commit -m "Your explanation of the changes goes here."
git commit -m "Title" -m "Long description goes here .........."; 
```

We can even configure git to open a text editor of our choice using:
``git commit``

## Good Commit Messages are Crucial!
Quality commit messages contribution to:
- **Traceability**: Commit messages clarify code history and aid in debugging.
- **Collaboration**: They help others understand the intentions behind changes.
- **Documentation**: They act as a form of source code documentation.
- **Change Management:** - "Change Logs" based on commits are often shipped with
each release.

### Bad Commit Messages:
- fixing stuff
- Final version.
- asdf

### Good Commit Messages:
- Enhance user experience by validating sign up form fields.
- Improve code readability by refactoring PlayerRegistrationService.
- Prevent null reference crashes by adding pointer checks in the teleport code.

