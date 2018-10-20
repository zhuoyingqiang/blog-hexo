---
title: win10上搭建hexo并发布到github上
date: 2018-10-14 23:03:01
modified: 2018-10-15 23:03:01
comments: true
tags:
- hexo
- github
categories:
- hexo教程
---

win10上搭建hexo，使用github发布
<!--more-->
# 起因
16年就搭建过一次，但是后面换电脑，源文件没有用git管理，后面也没怎么管，今天重新弄了一个，主要还是用到了几篇文章，记录下来以便参考.
希望通过这样来总结自己的技能。
# 教程
- [youmeek大神的教程-使用 Github 空间搭建 Hexo 技术博客--安装篇（基于 IntelliJ IDEA）](https://www.jianshu.com/p/1c98aed8d92e)
- [2018.5月使用Github+Hexo搭建自己的博客](https://blog.csdn.net/weixin_39879178/article/details/80319392)
- [hexo的基础用法](https://lfkid.github.io/2016/11/16/Hexo%E6%95%99%E7%A8%8B%EF%BC%9A%EF%BC%88%E4%B8%89%EF%BC%89%E4%BD%BF%E7%94%A8Hexo%E5%86%99%E5%8D%9A%E5%AE%A2/)
- [next主题官网](http://theme-next.iissnan.com/getting-started.html)
- [使用jekyll和hexo搭建免费博客](http://www.alonemonkey.com/2016/05/20/blog-by-jekyll-hexo/)
- [arccode](http://www.arccode.net/)
# 步骤
## 安装并且发布博客到git首页
这部分主要是根据youmeek大神和第二篇教程交叉到来看，搭建基本没什么难度。
### 需要注意两个地方
1. 两篇教程在设置npm源采用的方式不同，但是其实效果都一样，随便采用一种即可(个人倾向于第二篇那种)。
2. 设置全局git账号不是必须的，我按照第二篇文档提示输入
    
```
git config –-global user.name “55kaikainiubi”  //(“”的账号是刚才Github里面自己注册的账号) 
git config –-global user.email “836508484@qq.com” //(""的邮箱是你自己注册的邮箱
```
会被提示错误，直接不用配置，进行ssh的配置就行了。

## 将源码提交到git管理
这部分就是之前没有做的，这样做可以避免物理机问题导致又重新弄的尴尬。 这里面遇到了问题，就是下载主题的时候是直接git clone下来的，所以你源码里面直接push上你的git不行，需要先把主题中的git目录删除，要不然它会把主题模块提交到原作者git上，这个你肯定是提交不上去的。


# 后续
写一些自己正在学习的东西