---
title:  hexo发布到gitee pages码云上，同时托管到github和码云
date: 2018-10-20 22:07:00
comments: true
tags:
- hexo
- github
- gitee
categories:
- hexo教程
---

前一篇hexo写静态博客发布到github上托管，但是由于总所周知的原因，需要一个国内的。所以想到了用码云提供的类似服务来实现。
<!--more-->
# 起因
前一篇hexo写静态博客发布到github上托管，但是由于总所周知的原因，需要一个国内的。所以想到了用码云提供的类似服务来实现。

本来想用网上的教程，[类似于同时上传hexo到github和coding的方案](https://www.cnblogs.com/tengj/p/5352572.html)

## 发布到码云之后，页面显示不正确的问题
但是中间码云有个坑就是码云hexo生成的html必须发布到你代码项目目录下，也就是你的hexo项目根配置文件中需要配置：

```
root:/hexo_log/ #你的码云上的项目名称，而github这个路径设置为 / 也就是根路径就可以了
```
## 目前的发布方案
==所以我目前采用的方式是维护了两个不同分支源码，分别来推送到不同平台==
> 

平台|平台博客地址  | 源代码地址
--- | ---          |  ---
 github| http://zhuoyingqiang.github.io/ | https://github.com/zhuoyingqiang/blog-hexo/tree/master
gitee| https://zhuoyingqiang0624.gitee.io/hexo_log | https://github.com/zhuoyingqiang/blog-hexo/tree/gitee

# 教程
- [hexo+码云搭建个人免费博客](https://www.jianshu.com/p/b5cafa704613#gitee%E6%89%98%E7%AE%A1)
- [Hexo添加字数统计、阅读时长](https://www.jianshu.com/p/baea8c95e39b)

# 步骤
> 由于有了前一篇文档的基础，所以和安装部署到github流程是相似的，只是要主要发布目录的配置
    

# 后续
- 集成留言功能
- 集成站内搜索以及统计功能
- [静态图片的问题](https://www.jianshu.com/p/c2ba9533088a)