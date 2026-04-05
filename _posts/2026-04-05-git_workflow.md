---
layout: post
title: "Git Workflow"
date: 2026-04-05
categories: software
tags: [git, github]
---
## easier workflow
```zsh
> git checkout main

# do some editing

> git add ...
> git commit -m "..."
> git push -u origin main
```

## pull request workflow
``` zsh
> git checkout main

# update code from remote
> git pull origin main

# checkout new branch
> git checkout -b new_feature

# do some editing

> git add ...
> git commit -m "..."
> git push -u origin new_feature

# create and merge the pull request on Github

> git checkout main
> git pull origin main
> git branch -d newpost
> git push origin --delete newpost

> git checkout main

# update code from remote
> git pull origin main
```