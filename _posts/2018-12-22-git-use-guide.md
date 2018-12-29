---
layout:     post
title:      运维视角的Git使用及快速上手
subtitle:   介绍Git常用命令
date:       2018-12-22
author:     老麦
header-img: img/post-bg-rwd.jpg
catalog: true
tags:
    - git
    - devops
    - github
    - 分支
---
# 写在前面
对于习惯于通过shell、sqlplus来操控数据库的DBA来说，对github的印象也仅限于它被称为`世界上最大的同性交友网站`，大概知道git是个版本管理工具，而github作为全球最大的代码托管平台，程序员的最爱，上面有大量的开源程序和优秀资源。但版本管理工具多了，从vcs到svn，甚至直接重命名文件（文件夹）副本的方式来管理。。。一切的改变，也许就是从某次不经意注册了Github账号开始，然后search，fork，clone，还挺好玩...至此一发不可收拾。
# Git诞生
> git是一个分布式版本控制软件，最初由林纳斯·托瓦兹创作，于2005年以GPL发布。最初目的是为更好地管理Linux内核开发而设计。

上面这个来自wikipedia的关于git的介绍，就像是在说周末花两小时陪儿子看了一部动画片一样稀松平常。而事实上，Git诞生的历史就像科比的81分，或者麦迪的35秒13分一样，完全就是软件史上的`另一个`传奇（上一个传奇是Linux，也是Linus干的）。关于Linus在2005年花了两个星期用C完成Git开发，并用它来代替商业软件BitKeeper管理Linux代码的故事，请移步[这里](https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/00137402760310626208b4f695940a49e5348b689d095fc000)观看。
# Github和Gitlab

# Git快速上手
# 常用命令介绍

## git config 配置用户信息
> local:当前所在仓库 global：当前用户所有仓库 system：当前系统所有用户

* git config [--local | --global | --system] user.name 'xxx'
* git config [--local | --global | --system] user.email 'xxx'
* git config --list [--local | --global | --system]

## git init建立Git仓库
* 把已有项目纳入Git管理 git init
* 新建项目并纳入Git管理 git init your_project

## git commit
git commit -am'xxx'
## git log查看版本历史
git log --oneline
git log -n4 --oneline
git log --all
git log -n4 --oneline --all --graph
git help --web log
## git checkout
git checkout -b xxx commitid
## gitk图形界面查看版本历史 
# 几个容易混淆的概念
# 总结