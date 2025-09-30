---
title: History
parent: Git-Fundamentals 
nav_order: 1
---

<!-- prettier-ignore-start -->
# Configure Git 
{: .no_toc }

Before we create our repository we need to set up Git on our device. We need to set our main folder where your project will be stored. Next we need to give some info to git. This is handy when we need to see commit messages. 

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->
## Testing, Testing, 1, 2, 3...
Start by launching Git Bash from the Windows Terminal.
And try running:
``git --version``

Let's make a folder to play in:
```
mkdir my-first-git
cd my-first-git
```

## Configuring Git
Next, let's tell Git who you are. Git needs to know your name and email.
```
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```
Let's also turn on helpful colourization.
``git config --global color.ui auto``
You only need to set these once!