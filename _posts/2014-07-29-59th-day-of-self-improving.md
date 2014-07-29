---
title: "自我修炼第59天--后会无期，平凡之路"
layout: post
description: "我不好也不坏 不特别出众 我只是敢不同
我的人生就是 一错再错 错完了再重头
也许放弃掉一些 活得更轻松 我却不再是我
我不愿一生 晒太阳吹风 咸鱼也要有梦
—五月天《咸鱼》"
photo_url: "http://ffanson.qiniudn.com/FFAnson/gh-pageDSC06690.JPG-indexRectangle1"
comments: yes
---
![](http://ffanson.qiniudn.com/FFAnson/gh-pageDSC06690.JPG-indexRectangle1)


自我修炼来到了第59天，还有一天就两个月了，距离自我设定的期限还有35天，明天出发去成都九寨玩5天，回来刚好剩下最后一个月。离设定的期限越近，不免出现了焦躁和不安的情绪，竟然路已经走到了现在这里，最后或者再试一次吧，我想做有趣的事，我想成为有故事的人，我下了这个决定，还是先来点鸡汤歌词来打一下气吧：
> 我不好也不坏 不特别出众 我只是敢不同
我的人生就是 一错再错 错完了再重头
也许放弃掉一些 活得更轻松 我却不再是我
我不愿一生 晒太阳吹风 咸鱼也要有梦
—五月天《咸鱼》

最近看了韩寒导演的电影《后会无期》，貌似其实当导演也不是一件难事吧，但当初我却放弃了，不过已经不再重要了，我已经找到我要走的路了。我不是韩迷，但我一直都觉得韩寒是一个有自己想法，对生活敏感，对自己诚实的人。《后会无期》是他的处女作，先不论他在技术层面，电影语言上的运用如何，但我觉得他讲了一个不错的故事，也抛出了很多值得思考的问题。一千个人就有一千个哈姆雷特，一千个观众也会有一千个后会无期。对于电影抛出的问题我思考了很多，我并不准备在这里展开叙述，但有一个感触想在这里分享：每个人都走在一条平凡之路上，在这条路上会遇见很多擦身而过的人，他给你留下或深或浅的印记，这些交集会影响着你下一步的选择，你会成长，你会改变，但你一定要对自己诚实、勇敢和坚定，不然你只会成为别人故事里的配角，甚至是路人甲乙丙。

总结一下从上次文章到现在的学习，在这20多天里，主要有以下几个内容：

1. 巩固了CSS方面的知识，以前有很多知识点都是模模糊糊的，通过这次的学习，清晰了很多内容，也学到了之前不曾接触的，后文会展开记录；
2. 学习了一些web开发的小技巧，主要来自《web开发秘方》一书；
3. 了解了[移动端重构方面](http://www.w3cplus.com/blog/tags/429.html?page=1)的基础知识；
4. 对node.js进行了较为完整的学习；
5. 对BackBone.js框架有了初步的认识（BackBone.js的相关文章：[Backbone使用总结](http://www.pchou.info/javascript/2014/06/26/backbone-summary-01.html)，[Backbone first glance](http://press.mcfog.wang/2013/05/backbone-first-glance/)，[认识BackBone系列文章](http://blog.segmentfault.com/stephenlee/1190000000465965)）；
6. 对Angular.js框架进行较为基础的学习，因为接下来的项目将会使用上，（Angular.js学习资料：[七步从Angular.JS菜鸟到专家系列文章](http://blog.jobbole.com/46779/)，[Build custom directives with AngularJS](http://www.ng-newsletter.com/posts/directives.html)，[shaping-up-with-angular-js](http://campus.codeschool.com/courses/shaping-up-with-angular-js/intro)）后文展开记录；
7. 对Hybrid App的框架Framework7，ionic和onsenUI进行了技术选型，搭建好了phonegap的开发环境（phonegap开发环境的搭建可以参见如下两篇文章：[Mac 10.9x下安装配置phonegap3.0开发环境 (涉及android sdk配置)](http://www.cnblogs.com/willian/p/3516613.html)和[PhoneGap 3 CLI Setup on Mac & Windows](http://thejackalofjavascript.com/phonegap-3-cli-setup-mac-windows/)）。

一、关于CSS方面的学习记录
以下记录是《CSS设计指南》的学习笔记，相关章节也是书中的章节
1. 第2章：（1）特指到最明确的元素样式，为最终计算显示样式，ICE计算特指值；（2）::after和::before为元素为默认在指定的元素增加inline类型的子元素，可修改为block属性或inline-blockline属性。
2. 第3章：（1）float令子元素特破了父元素的包裹，浮至父元素的左上端或右上端，其他同级元素在父元素的大小内尽力与浮动元素并排，父元素继续包裹其他子元素。（2）没有显示设定宽度的block元素总宽度（外边距+边框+内边距+内容）与父元素等宽；若设定则是设定了元素的内容宽度。（3）理解好定位元素的上下文；（4）color是前景色，默认影响边框颜色，background-color后景色；（5）前景-背景-背景颜色，背景范围默认包括外边距，通过background-clip设置；（6）多背景通过逗号分隔每一层图片设置。
3. 第4章：（1）字体相对大小用em时，通过逐层计算父元素大小继承，基本是body为首先基础，1em为16像素，如不对父元素设置绝对大小，则每一个子元素相同的em值对应的像素值不等；（2）text-indent直接继承父元素的计算缩进值；（3）文本属性默认只对文本或inline元素有影响，因文本内容有一个inline-box包裹，不可设置高度和宽度，line-height是设置一行inline-box的高度，与字体大小相互作用影响行间距；（4）text-align设置文本水平对齐位置，center属性值并可设置在有固定宽度且较小的元素和图片；（5）vertical-align只对行内元素有影响；（6）fontssquirrel.com转换字体格式，用于@font-face引入。
4. 第5章：（1）960px的width是最理想的；（2）box-sizing改变盒子的宽度计算范围（3）max-width控制包含元素的宽度；（3）display：table-cell。
5. 第6章：（1）父元素 子元素 + 子元素选择法；（2）表单<label>可包含控件也可不包含，用for来默认对应id；（3）表单legend元素的定位机制不明，在入面嵌入<span>来控制定位，再设定为block；（4）transition属性跟踪相关属性变化的过渡，实现搜索框的变化；（5）<figcaption>在<figure>中必须是唯一的，并且是第一个子元素或最后一个子元素；（6）行内元素的定位基准为文本基线；（7）z-index对除static之外的元素有效；（8）使用border及::before和::after形成三角形。
6. 第7章：（1）没有宽度的元素水平居中，父元素为text-align:center，子元素为display:inlineblock；（2）垂直居中，文本line-height与父元素同高，为display:row,vertical-align:middle(middle只对单元格有效)；（3）inline-block外边距不能为auto。

二、关于HybridApp应用的框架选型

HybridApp是采用HTML5技术开发通过Phonegap等相关工具打包成类NativeApp的应用，其特点是采用前端语言进行开发，一次开发跨平台部署，但却是以牺牲应用性能为代价，用于相关开发的框架现在比较多，如jQueryMobile，senchaTouch等，但通过网上资料显示，这两个框架优化并不是特别好，目前较为流行的有以下三个：Framework7，ionic和OnsenUI，下文从文档，学习成本，社区，跨平台性，component和其他特性六个方面进行比较：

1. 文档：三个框架都具备较为完整的文档，通过文档学习起来并没有太大问题，估计Framework7框架出现得较为晚，所以文档方面仍在不断更新；
2. 学习成本：Framework7并不具备MVC的模式，就像普通的webapp框架，学习成本较低；ionic和OnsenUI比较依赖AngularJS，采用MVC模式，比较适合用于应用类型的开发，但学习成本较高；
3. 社区：ionic的社区较为活跃，Framework7和OnsenUI相对欠缺；
4. 跨平台性：Framework7主要针对的是iOS平台，虽然也可用于Android平台，但考虑到Android平台的混乱，支持效果不可保证；另外两者都号称对于android平台有不错的支持并且支持Android2.3以上；
5. component：只能说三者都有足够使用的component；
6. 其他特性：OnsenUI有个在线的IDE monaca，并且支持直接在移动设备上Debbug，但经过试验可以支持另外两种框架；OnsenUI还有个主题自定义工具。

三、关于AngularJS学习的记录

关于Angular学习方面，上面已经记录了我的相关学习资料，现在讲讲我的一些理解：

1. angular的适用范围是针对那些AngularJS是一个 MV* 框架，最适于开发客户端的单页面应用。它不是个功能库，而是用来开发动态网页的框架。它专注于扩展HTML的功能，提供动态数据绑定（data binding），而且它能跟其它框架（如jQuery）合作融洽。如果你要开发的是单页应用，AngularJS就是你的上上之选。Gmail、Google Docs、Twitter和Facebook这样的应用，都很能发挥AngularJS的长处。但是像游戏开发之类对DOM进行大量操纵、又或者单纯需要极高运行速度的应用，就不是AngularJS的用武之地了。
2. 使用好angular系统定义的directive，每一个directive都可以理解成一个功能区域，都是一个controller和view的绑定；
3. 利用自定义的directive来简化应用架构；
4. 使用好$scope service来设定数据的有效范围；
5. 使用serveice概念来扩充controller的功能，并实现controller间的数据共享；
6. 忘记对DOM的操作；
7. 表达式对于数据的展现功能；

接下来，将会以开放一个应用来结束这次的修炼，作为期末考试。抓紧和珍惜剩下的时间。然后开始一次新的尝试。