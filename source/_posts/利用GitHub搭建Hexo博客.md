---
title: 利用GitHub搭建Hexo博客
date: 2018-01-23 10:05:39
tags: [建站,Hexo]
categories: 建站
keywords: 博客,建站,Hexo,GitHub Pages
---

# 前言

> 这是我用自己建立的博客写的第一篇文章，本着开源的思想，本篇博客主要介绍下，我是如何一步步新建了这个博客网站，供各类人士参考。此篇博客我是站在专业IT人士的角度去编写的，所以看不懂的地方在评论中提出，我会尽量解答。由于我是利用零碎的时间写的博客，所以更新比较慢，请见谅。



[我的博客地址](https://zhshqo.github.io/)

[我的博客源码地址](https://github.com/zhshqo/zhshqo.github.io)

{% asset_img 测试图片.png 文章的第一张图片测试用 %}



# nodejs 的安装

Nodejs的下载地址：

<http://nodejs.cn/download/>

安装时一路默认即可，这个安装会把nodejs和npm配置到系统PATH中，这样在命令行的任何位置都可以直接用node执行nodejs，用npm执行npm命令。

检查nodejs是否安装成功可以这样查看：

{% asset_img node-v.png node-v %}

另外，因为可能的GFW问题（不然会下载很慢很慢，也可能下载失败），所以建议把npm的仓库切换到国内taobao仓库，执行下面的命令（我当前采用的方式）：

```bash
npm config set registry "https://registry.npm.taobao.org/"
```

还有一种方式，注册cnpm命令，如下：

```bash
npm install -g cnpm--registry=https://registry.npm.taobao.org
```

 

配置后可通过下面方式来验证是否成功

```bash
npm config get registry
```

{% asset_img npm_config.png npm_config %}