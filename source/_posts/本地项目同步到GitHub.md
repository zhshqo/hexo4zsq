---
title: 利用GitHub搭建Hexo博客
date: 2018-01-23 10:05:39
tags: [建站,Hexo]
categories: 建站
keywords: 博客,建站,Hexo,GitHub Pages
---



> 本文的意图在于介绍如何将本地的项目文件夹同步到GitHub上



# 在GitHub上新建远程仓库



注意：新建的仓库名称最好与本地项目文件夹的名称一致

这次以我的博客项目hexo4zsq为例

![QQ截图20180126104513](D:\workspace_nodejs\hexo4zsq\source\_posts\本地项目同步到GitHub\QQ截图20180126104513.png)

点击Create repository即可完成创建

![QQ截图20180126105124](D:\workspace_nodejs\hexo4zsq\source\_posts\本地项目同步到GitHub\QQ截图20180126105124.png)

记录以上git地址备用

# 初始化本地仓库

打开CMD命令窗口，CD到我们的项目文件夹

```bash
cd D:\workspace_nodejs\hexo4zsq>
```

接着运行以下命令初始化本地仓库

```bash
git init
```

效果如下

![QQ截图20180126105500](D:\workspace_nodejs\hexo4zsq\source\_posts\本地项目同步到GitHub\QQ截图20180126105500.png)

添加远程push地址

```bash
git remote add origin https://github.com/zhshqo/hexo4zsq.git
```



# 将本地仓库与git远程仓库关联

先将远程仓库和本地仓库合并

``` bash
git pull origin master --allow-unrelated-histories
```

然后提交本地仓库到远程仓库

``` bash 
git push origin master
```

