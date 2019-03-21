---
title: hexo搭建博客详细教程
date: 2019-02-28 16:46:59
tags:
  - hexo
  # - 测试2
categories: 教程
---

### 前言

一个偶然的机会，想自己搭建一个博客，在网上查了很多，最后决定用 hexo + github page，搭建后可以不到github上面直接编译成为静态文件，配置github page即可线上访问，无需购买域名，欢迎来访 [好记性不如烂键盘](https://zhi-he.github.io/blog)。
我是一个前端菜鸟，感觉这个比较适合我，走了很多弯路，本着服务大众的态度，写下这个教程，第一次写博客，欢迎吐槽。
> 注：本教程只适用于windows系统

### 搭建前准备

1. [nodeJs](http://nodejs.cn/download/ "下载")
2. [git](https://git-scm.com/download/win "下载")
3. 编辑工具（[VSCode](https://code.visualstudio.com/Download "下载") 或 其他）
   
### 开始搭建

使用npm安装hexo脚手架，之前一直使用cnpm安装，后来发现cnpm有些意料之外的bug，决定使用npm，把源地址换为cnpm即可，在此推荐一个工具 `nrm`，`nrm`是npm源地址管理工具，直接`npm install nrm -g`安装，`nrm use cnpm`即可切换完成。

#### 一、全局安装hexo脚手架

```
npm install -g hexo-cli
```

#### 二、初始化

```
hexo init myBlog
cd myBlg
npm install
```
这时你看到的应该是这样
{% asset_img 2019-03-10-23-39-02.png image %}

