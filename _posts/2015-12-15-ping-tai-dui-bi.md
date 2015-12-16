---
layout: post
date: 2015-12-15 18:59:45 +0800
title: 各种搭建博客平台程序的对比
tags: git github wordpress hexo jekyll
categories: 技术 
---

**1、Wordpress**    
搭建平台PHP+MYSQL：     
* 优点：搭建简单，功能强大，插件及主题模板资源非常多，备份简单，支持转到多种其它博客程序；      
* 缺点：程序越变越臃肿，且需在线编辑文档（在线编辑的一个问题就是需排版，而且写作时不小心刷新就会丢失文档）。wordpress已经看起来越来越不像是一个博客了，更像是一个CMS。   

**2、Jekyll**   
使用Ruby语言，搭建平台Ruby+devkit+gem，如果使用博客的代码高亮用到了Python的Pygments模块，则需再安装Python；  
* 优点：主题模板较多，支持markdown、liquid以及原始的html、css， 可直接在github上搭建， 继承github上的各种好处（版本控制，免费，无流量限制）；    
* 缺点：安装相对复杂（使用jekyllbootstrap框架安装则相对简单，不过不支持windows下搭建），仅仅适合小型网站，不适合大中型网站；    
即是优点也是缺点是它生成的是静态页面无法实现动态加载，不需要额外的数据库（不方便数据搜索）。    

**3、Octopress**    
基于Jekyll，同样使用Ruby实现，搭建平台Ruby+devkit+git，如果使用博客的代码高亮用到了Python的Pygments模块。其优缺点与Jekyll类似。    

**4、Hexo**   
出自台湾大学生tommy351之手，是一个基于Node.js的静态博客程序，其编译上百篇文字只需要几秒。hexo生成的静态网页可以直接放到GitHub Pages，BAE，SAE等平台上。相比Jekyll，它隐藏了很多命令，使得搭建博客非常简单。现在模板也越来越多。    
* 优点：搭建简单，生成速度快。    
* 缺点：异地发布的问题，网上有相应的解决方案“hexo服务器端布署及Dropbox同步”、“利用Github和Heroku远程发表hexo文章”，“自制node.js + npm绿色版”。

**5、Ghost**    
构建于Node.js，模板众多。本质上跟WordPress一样（btw, 其创始人以前是在WordPress工作的），无法构建在虚拟主机上，需要vps或服务器。如果你厌烦了手工安装Node.js和Ghost，可以试试BitNami团队开发的Ghost安装工具，它提供了对所有主流平台的支持。
* 优点：使用ghost有一个好处只要能上网就可以写博客，在线写作支持markdown（左边是markdown右边可以看到预览效果），后台管理简单，并且有很多非常漂亮的模板可供选择。    
* 缺点：需要VPS或独立的服务器，博客无法实现Archives及Categories显示，只能通过Tags。
[链接](http://read.mobi/2015/03/15/blog-source-comparison/)
