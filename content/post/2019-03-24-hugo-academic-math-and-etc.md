---
title: 好多坑，Hugo,academic, math and etc...
author: 沈家铭
date: '2019-03-24'
slug: hugo-academic-math-and-etc
categories:
  - 随笔
tags: []
image:
  caption: ''
  focal_point: ''
---

随便选了这个模板来从头构造博客。
一开始无法render \$$下的latex代码，不知道为啥，一检查发现连网页中都没有mathjax的js代码。遂去tutorial里面关于latex math formula [那一节](https://sourcethemes.com/academic/docs/writing-markdown-latex/#rm-latex-math) 去找，发现没有说，只是说怎么在markdown里面写。最后是在issue里面找到别人提过一嘴，要在在config里面加math=true。。。真坑
加完了还不算完事，公式有一多半显示不了，一看是符号_有问题，改成 _ 以后还有begin{aligned}有问题，omg，因为这是hugo版本的latex render，和pandoc以及其他的亚语法有区别，感觉碰到了大坑orz。所以估计，还得换或者再深入了解一下怎么办再说吧。。。

第二个坑是在用Rstudio的addin，new post里面提示
> Error: Unable to find theme Directory: /Users/wglaive/Documents/GitHub/Blog_restart/themes/academic

一看文件夹，template的名字叫hugo-academic....orz，直接暴力尝试复制hugo-academic并且重命名为academic，然后就在写这篇。。。希望能成功搞定吧。
