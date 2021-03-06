---
title: "自我修炼第36天--Anson的博客换了个门面"
layout: post
description: "因为我的博客定位就是一个记录和阅读的工具，所以这次的更新集中在版面美观和减少不必要的元素避免分散阅读的注意力的优化上"
photo_url: "http://ffanson.qiniudn.com/FFAnson/gh-pageblogDraft.jpg-indexRectangle1"
comments: yes
---
![](http://ffanson.qiniudn.com/FFAnson/gh-pageblogDraft.jpg-indexRectangle1)

在写今天的文章之前，我想向大家介绍我用来写文章的Markdown工具。Markdown是一款十分轻量的标记语言，它轻量到足以让你可以将写作的注意力就集中在写作上，关于Markdown更加详细的介绍和相关的工具在网上有十分多，搜搜就是了。而我用于写作的Markdown工具是一款webAPP，叫做[作业部落Cmd Markdown](http://www.zybuluo.com),无需安装，云保存和同步，你点一下就知道有多好的。今天是作业部落发布第八次更新，也是我的博客的第一次更新。今天就谈谈这次我博客更新的感受和经验。话说两天更新一个博客还真有点慢，差太远了。

题图是我的预设草稿和最终实现的效果，跟预想还是有出入的。这次的更新主要有以下几点：

- icon由方形换成了圆形；
- 增加了苹果移动设备上的添加至主屏幕图标；
- 使用七牛优化了图片，降低了图片的大小，加速了文档的加载加载；
- 更换了全局版式和文章页版式，删除了主页文章索引上的图片，突出了文章内容；
- 文章页的导航条可自动隐藏；
- 使用了[层叠字体](http://www.webdesignerdepot.com/2014/06/how-to-get-started-with-layer-fonts-in-css/)；

因为原来博客的主题是下载下来的，而且没有相应的说明文档，再加上技术上的不熟练，使得在这次这么大动作的优化下，占用了较长的时间。在这次的优化过程中，主要遇到了两个问题：

1. 元素定位，并在不同浏览器和移动设备上的兼容问题，健壮性不够，如在OX平台上safari和chrome渲染出来的边距有差异，耗费了很多时间在该问题上的调试，最终的解决方案也不够优雅；
2. 移动设备上的响应布局，在解决该问题上主要用了viewport和media query的方法，在台式设备上适应不同的浏览器视窗大小，meidiaquery应该使用min/max-width,在移动设备上用的是min/max-device-width进行相应的响应布局，并且可以使用zoom进行viewport的缩放。据说[froont](http://froont.com/)是一个在线的可视化响应布局神器，下次可以试试使用。

因为我的博客定位就是一个记录和阅读的工具，所以这次的更新集中在版面美观和减少不必要的元素避免分散阅读的注意力的优化上，但仍有很多细节问题需要继续优化，目前主要有以下两个问题：

1. 字体大小和选择上影响了阅读的感受，特别在移动设备上，未经过处理，导致标题字体过大，十分不美观；
2. 在文章页面上的导航条自动隐藏效果不佳；

坚持和不断优化吧，骚年！