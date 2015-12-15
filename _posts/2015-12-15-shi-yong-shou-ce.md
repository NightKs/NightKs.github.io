---
layout: post
date: 2015-12-15 13:45:20 +0800
title: git使用手册
categories: 技术 手册
tags: 手册 git github
---
#git

常用命令

	git pull	//更新远程仓库的内容到本地
	git add .
	git commit -a -m "加改动信息"		//添加到暂缓区
	git remote add origin https://github.com/(github用户名)/(jekyll项目名称).gi		// 上传到本地库
	git push -u origin maste		//更新本地库内容到远程仓库

**注意**

* 工作目录：git clone 后获得的一份本地的代码，也包括新编辑的，尚未加入版本控制的代
* 暂存区域：git add 后暂存起来，尚未 git commit 的代码
* 本地仓库：git commit 后正式被版本控制记录起来的代码

**教程:**1.[Git 常用命令用法：程序员的场景](http://pm.readthedocs.org/zh_CN/latest/vcs/git/usage.html)2.[史上最浅显易懂的Git教程！](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)3.[Pro Git（中文版）](http://git.oschina.net/progit/)
#github

**教程:**1.[版本控制入门 – 搬进 Github](http://www.imooc.com/learn/390)

#jkl
这是一个nodejs写的在命令行下使用jekyll的工具，可以帮助大家减少一些重复操作。[使用jekyll-cli快速写blog](http://jser.me/2014/03/25/%E4%BD%BF%E7%94%A8jekyll-cli%E5%BF%AB%E9%80%9F%E5%86%99blog.html)。
安装过nodejs之后，可以用下面的命令来安装

	$ npm install -g jekyll-cli
安装完成后，使用jkl命令就行了。如：

	//新建名为“使用jekyll-cli快速写blog”的文章
	$ jkl post 使用jekyll-cli快速写blog
正常的情况下它就会在**_post**目录创建好一个文件名是**使用jekyll-cli快速写blog**的markdown文件，同时这个文件的内容已经写上了时间标题，如果你不想使用中文的文件名，可以加上**-p**参数，它会帮你把中文转换为拼音

	$ jkl post -p 使用jekyll-cli快速写blog
更多详细的用法，可以查看帮助**$ jkl -h**子命令的详细用法，可以同样可以查看帮助，比如查看**post**的详细用法和参数**$ jkl post -h**
