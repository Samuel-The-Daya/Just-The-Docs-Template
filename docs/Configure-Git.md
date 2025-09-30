---
title: History
parent: Git-Fundamentals 
nav_order: 1
---

# Configuring Git
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