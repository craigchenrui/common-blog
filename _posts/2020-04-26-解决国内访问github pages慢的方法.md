---
layout:     post   				    # 使用的布局（不需要改）
title:      解决国内访问github pages慢的方法（仓库私有化） 				# 标题 
subtitle:      Blog                #副标题
date:       2020-04-26 				# 时间
author:     陈锐CR 						# 作者
preview-img: "/img/github page.png" 		          # 预览图
header-img: img/post-bg-dutme.jpg 	#这篇文章标题背景图片
catalog: true 						# 开启catalog，将在博文侧边展示博文的结构
istop:   true          # 设为true可把文章设置为置顶文章
music-id:         # 网易云音乐单曲嵌入
music-idfull:         # 网易云音乐歌单嵌入
apserver:     # 音乐平台netease/tencent/kugou/xiami/baidu
aptype:     # 音乐类型song/playlist/album/search/artist
apsongid:     # 音乐song/playlist/album id
tags:								#标签
    - Blog
---
## 解决国内访问github pages慢的方法（更新）

在很多时候，我发现我在访问我的博客时，非常缓慢。这将很影响我的浏览体验，GitHub pages是GitHub提供的一项静态站点托管网页，由于国内因为某墙的问题，访问延迟200-300ms，当然这还是在网络较好的时候，在网络差的情况下会很难加载完全网页，异常烦躁。于是，我开始搜索相关教程，决定解决这个问题。

![](https://tva1.sinaimg.cn/large/00831rSTgy1gditcpz3xaj31rr0u0gp1.jpg)

### 第一种方法：减少图片素材的本身大小

在加载过程中，很多时间是图片加载缓慢，可以通过图片压缩工具进行减少容量，我使用的是[**Mac imageoptim**](https://imageoptim.com/mac)



### 第二种方法：科学上网方法（我再这里不细说，会用的人都懂的）



### 第三种方法：使用CDN为网站加速。

CDN是什么？CDN的全称是Content Delivery Network，即[内容分发网络](https://baike.baidu.com/item/内容分发网络/4034265)。CDN是构建在现有网络基础之上的智能虚拟网络，依靠部署在各地的边缘服务器，通过中心平台的负载均衡、内容分发、调度等功能模块，使用户就近获取所需内容，降低网络拥塞，提高用户访问响应速度和命中率。CDN的关键技术主要有内容存储和分发技术（摘自百度百科）。

国内的CDN要么收费，要么就是网站要备案。

更新：可使用[cloudflare](https://www.cloudflare.com/)进行免费的cdn加速，服务器在美国。

这部分，我也参考了[**运维咖啡吧的博客内容**](https://www.cnblogs.com/37Y37/p/12551839.html) 使用Netlify进行加速，这也是我的备用网址之一，访问网址：[**Chen Rui  Blog**](https://chenrui.netlify.com/) ，然而并没有什么用，延迟还是很高。

![](https://tva1.sinaimg.cn/large/00831rSTgy1gditsqbcd9j31qx0u0q6m.jpg)



### 第四种方法：双重布局在国内的coding和国外的GitHub上。

对于国外GitHub上布局pages的方法：可参考[**柏荧的博客教程**](https://www.jianshu.com/p/e68fba58f75c)，我的博客是在此基础上进行的无数次的修改的。



国内coding布局：

在网络上有大量的教程，教你如何从GitHub上迁移到coding上，我参照的教程将 [**Jekyll 博客同时托管在 Github Pages 和 Coding Pages**](https://10101.io/2018/09/18/Blog_3)  和[**coding生成静态网址手册**](https://help.coding.net/docs/devops/cd/static-website.html#pageTitle)，需要注意的几点，1、电脑上需要安装git，2、注册coding账号，记住选择第三个DevOps项目。上传完代码库后，立即部署将会生成博客的网址，我的博客网址https://k2pvcm.coding-pages.com/ ，我再次ping了一下地址

![](https://tva1.sinaimg.cn/large/00831rSTgy1gdiow5ejj6j30sm0agwha.jpg)



这个访问网址快了好几倍。

更新，最近又发现一个很有用的免费托管平台，[**zeit**](https://vercel.com/)可以直接连通GitHub的仓库进行博客部署，自带cdn加速，服务器在台湾，对于国内的访问不错。直接关联GitHub中的博客项目，然后将自定义的域名链接到这个平台上，就可以把GitHub中的博客仓库私有化了，这将是对写作者来说非常有利的地方。



### 最后，我还是需要说明一点。

我已经弃用GitHub page，但可以通过我的私有网址进行访问博客**[https://7988888.xyz/**](https://7988888.xyz/)，这个将会是我第一时间更新和维护的博客网址。



coding pages的网址[**http://k2pvcm.coding-pages.com/**](http://k2pvcm.coding-pages.com/)，这个是国内访问更快速的网址，更新文章会慢些。



netlify pages的网址[**https://chenrui.netlify.com/**](https://chenrui.netlify.com/)，这个是和GitHub博客仓库同步更新的，也是为了防止GitHub page随时被禁止的可能访问网址。



zeit page的网址

- [https://chenrui-cf8jgd5tj.now.sh](https://chenrui-cf8jgd5tj.now.sh/)
- [https://chenrui-hazel.now.sh](https://chenrui-hazel.now.sh/)
- [https://7988888.xyz](https://7988888.xyz/)
- [https://chenrui.craigchenrui.now.sh](https://chenrui.craigchenrui.now.sh/)
- [https://chenrui-git-master.craigchenrui.now.sh](https://chenrui-git-master.craigchenrui.now.sh/)



----------

### 谢谢大家观看，如有帮助，来个喜欢或者关注吧！

----------

 本文作者：Chen Rui

 博客地址   ： [Chen Rui Blog][1] <br>
 知乎地址   :  [知乎专栏][2] <br>
 B站地址   :  [B站主页][3] <br> 书店地址   :  [书店主页](https://j.youzan.com/S8UKli)<br> 网易云音乐地址   :  [音乐主页](https://music.163.com/#/user/home?id=269228201)

[1]: http://7988888.xyz/
[2]: https://www.zhihu.com/people/braintechnology
[3]: https://space.bilibili.com/328549846

