---
title: hexo搭建博客详细教程
date: 2019-02-28 16:46:59
tags:
  - hexo
  # - 测试2
categories: 教程
---

### 前言

一个偶然的机会，想自己搭建一个博客，在网上查了很多，最后决定用 hexo + github page，搭建后可以不到github上面直接编译成为静态文件，配置github page即可线上访问，无需购买域名，欢迎来访 [一介码农](https://zhi-he.github.io/blog)。
我是一个前端菜鸟，感觉这个比较适合我，走了很多弯路，本着服务大众的态度，写下这个教程，第一次写博客，欢迎吐槽。
> 注：本教程只适用于windows系统

### 搭建前准备

1. [nodeJs](http://nodejs.cn/download/ "下载")
2. [git](https://git-scm.com/download/win "下载")
3. 编辑工具（[VSCode](https://code.visualstudio.com/Download "下载") 或 其他）
   
### 初始化基本博客

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

#### 三、运行

执行命令`hexo s`，此时，最基本的博客环境已经搭建完成

{% asset_img 2019-03-31-13-01-02.png image %}

打开 [http://localhost:4000](http://nodejs.cn/download/ "")，看到的页面如下

{% asset_img 2019-03-31-13-06-50.png image %}

#### 配置博客基本信息

网站基本配置基本信息，主要配置的是系统配置，官网已经做了详细说明，我再此不在说明

{% asset_img 2019-04-15-16-39-58.png image %}

配置部署配置`deploy`字段，我部署的站点是git默认的，`type`填`git`，`repo`是项目地址，`branch`是编译后的分支名称

{% asset_img 2019-04-15-17-15-22.png image %}


### 使用主题

博客搭建好后，默认使用的`landscape`主题，想要更换主题，只需在`themes`导入主题文件后即可，配置`_config.yml`文件即可，[官网主题](https://hexo.io/themes/)有很多，试了几个，但是还是`next`主题是最完善的，下面主要说一下`next`的使用

#### 安装主题

执行以下命令将主题文件下载至项目中

```
git clone https://github.com/theme-next/hexo-theme-next themes/next
```

看到以下结果，说明主题已经导入成功

{% asset_img 2019-04-15-16-28-43.png image %}

修改项目的`theme`字段，使用主题`next`，编辑后看到如下结果

{% asset_img 2019-04-15-17-35-12.png image %}

### 部署

登录github，在`settings`->`GitHub Pages`配置域名，即可访问。


