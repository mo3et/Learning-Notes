---
title: Git Docs
tags: ["Git"]
---

# Git Help

### 如何Clone所有Branch

git branch -a  查看远程分支，例如：  
remotes/origin/main  
remotes/origin/week1  
选择要的分支  
-  git checkout -b  《branch name》<branch>  origin/<barnch>《branch name》  （Branch例如是week1）

--------
All tips:
1. 找一个干净目录，假设是git_work
2. cd git_work
3. git clone http://myrepo.xxx.com/project/.git ,这样在git_work目录下得到一个project子目录
4. cd project
5. git branch -a，列出所有分支名称如下：
remotes/origin/dev
remotes/origin/release
6. git checkout -b dev origin/dev，作用是checkout远程的dev分支，在本地起名为dev分支，并切换到本地的dev分支
7. git checkout -b release origin/release，作用参见上一步解释
8. git checkout dev，切换回dev分支，并开始开发。
---------
