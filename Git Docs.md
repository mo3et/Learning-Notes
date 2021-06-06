---
title: Git Docs
tags: ["Git"]
---

# Git Help

- 查看本地分支和跟踪情况

> `git remote show origin`

- 清除多余分支

>  `git remote prune origin`

- 刷新分支列表

> `git remote update origin --prune`

- 删除远程已经merge的branch

> `git push origin --delete  <branch>` <branch>为具体的分支名

-------------

#### 如何Pull其他Branch

git branch -a  查看远程分支，例如：  
`remotes/origin/main  
remotes/origin/week1`  
选择需要Pull的分支  

`git checkout -b  <branch>  origin/<barnch>`  （Branch例如是week1）
