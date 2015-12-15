---
layout: post
date: 2015-12-14 23:21:29 +0800
title: jkl命令
tags: [jkl,手册]
categories: 手册
---
熟练一下markdown.
这是一个nodejs写的在命令行下使用jekyll的工具，可以帮助大家减少一些重复操作。[使用jekyll-cli快速写blog](http://jser.me/2014/03/25/%E4%BD%BF%E7%94%A8jekyll-cli%E5%BF%AB%E9%80%9F%E5%86%99blog.html)。
安装过nodejs之后，可以用下面的命令来安装


	$ npm install -g jekyll-cli
安装完成后，使用jkl命令就行了。如：

###新建文章命令

	//新建名为“使用jekyll-cli快速写blog”的文章
	$ jkl post 使用jekyll-cli快速写blog
正常的情况下它就会在**_post**目录创建好一个文件名是**使用jekyll-cli快速写blog**的markdown文件，同时这个文件的内容已经写上了时间标题，如果你不想使用中文的文件名，可以加上**-p**参数，它会帮你把中文转换为拼音

	$ jkl post -p 使用jekyll-cli快速写blog
更多详细的用法，可以查看帮助

	$ jkl -h
子命令的详细用法，可以同样可以查看帮助，比如查看**post**的详细用法和参数

	$ jkl post -h