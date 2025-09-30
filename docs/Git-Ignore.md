---
title: History
parent: Git-Fundamentals 
nav_order: 5
---

# Git Ignore 
## Not Every File Should Be Included
Sometimes there are files you don't want to include in your repo:
- Files that include secrets like passwords or API keys.
- Temporary files and folders.
- Build files and folders.
- Hidden OS files like .DS_Store (Mac) or Thumbs.db (Windows) files.

## Git Ignore File
Exclude files and folders by create a .gitignore file in the project root:
```
# Ignore specific files. (Note that comments start with: #)
Thumbs.db
# Wildcards: Ignore all .exe files.
*.exe
# Exception to wildcards: Do track the special.exe file.
!special.a
# Ignore all files in any folder called build.
build/
# Ignore all .pdf files in the doc/ folder and any of its sub-folders.
doc/**/*.pdf
```