---
layout:     post
title:      github搭建个人博客
subtitle:   最简洁明了的github博客教程
date:       2018-04-05
author:     Shaun
header-img: img/post-bg-github.jpeg
catalog: true
tags:
    - 水文
    - 博客
    - 教程
    - github pages
---

## 起因

清明节吃饱了没事干，想起自己一直想搞个个人博客。现在，加上最近想系统的刷一下OJ，并记录下来。因此，是时候了，搭建一个博客并记录OJ和其他学习过程。

选择博客：其实自己之前就有几个csdn账号，也有WordPress。其他的选择还有博客园，简书，github等等等等。我自己只有一个快过期的腾讯云服务器，域名也过期了不想续费，WordPress上不想写技术相关的东西。嗯，因此，就决定是github了，高度可定制，另外，我的github也该是时候活动一下了。

（觉得自己的github用户名太长，重新申请了一个zryang）

最快速版本请拉到最后。

#### step1

在自己的个人页面新建一个repo

![新建repo](https://i.loli.net/2018/04/05/5ac5f9357d453.png)

#### step2

给这个repo取名为：<username>.github.io，其中<username>替换成你的github账户名，如我的github账户名为zryang，则为zryang.github.io，初始化README。

![初始化repo](https://i.loli.net/2018/04/05/5ac5f9ba50b4d.png)

#### step3

进入该repo，点击Settings

![Settings](https://i.loli.net/2018/04/05/5ac5fa029041c.png)

#### step4

在Settings中下拉，找到GitHub Pages，选择Source为master branch，点击Choose a theme，选择一个博客主题

![Github pages](https://i.loli.net/2018/04/05/5ac5fa51b33fd.png)

#### step5

选定博客主题后，点击Select theme

![select theme](https://i.loli.net/2018/04/05/5ac5fa91dca32.png)

#### step6

第5步后，页面会跳转。下拉，Commit changes

![commit](https://i.loli.net/2018/04/05/5ac5facb0b342.png)

#### step7

在地址栏输入：用户名.github.io，进入博客主页。

![success](https://i.loli.net/2018/04/05/5ac5fb0cb9c3c.png)

至此，github pages的博客基本搭建完成。
之后，在根目录新建index.html,即是博客主页。

## Notes

#### 为什么要将repo取名为：用户名.github.io

这样取名的好处是，当你在地址栏输入：用户名.github.io时，进入的就是你的博客首页。

否则你的博客首页就是：用户名.github.io/repo名/

而输入地址：用户名.github.io/ 时，会404

具体的博客地址以Setting---Github Pages---your site is 为准

## 最快版本

* step1 新建github账号

* step2 fork别人的博客repo

* step3 修改Settings

* step4 编写发布自己的博客

#### 要点1：博客模板

自己白手起家的博客，要搞得好看顺心，非常麻烦。最好的办法就是直接fork别人配置好的博客，并在其基础上进行修改。github的博客是以github pages为基础的静态页面，主要建站工具有Jekyll和Hexo，两者都提供有非常丰富的工具和模板，也有很多博主做了非常好看的博客，在初入坑时完全不需要自己重复造轮子。

我参考的是[黄玄](https://github.com/Huxpro/huxpro.github.io)和[柏荧](https://github.com/qiubaiying/qiubaiying.github.io)两位的模板，两位风格好像是一样的，我不知道孰先孰后，在此一并谢过。

此外在[jekyllthemes](http://jekyllthemes.org/)也可以找到很多模板。只是我之前试了一下，找的几个好像解析不出来，不知道是什么原因。

此外，可借助万能的google，国内就用万能的百度吧。以“github pages 模板”为关键词搜索，能搜出一大堆。只是要自己去啃去配置。

当然，最简单的方法还是万能的github，多找几个博主的博客看看，喜欢哪个就fork哪个，自己再慢慢修。


#### 要点2：修改Settings

把别人的博客fork过来后，有些地方需要修改。

**1** 首先需要Repository name里面的用户名改成自己的用户名。

**2** 对应的，Github Pages中，Your site is published at后面的地址也会变成你自己的。

**3** 修改库根目录下的CANME，这个文件是绑定域名用的，如果有个人域名，就改成自己的域名，没有就删除。

**4** 其他更细致的东西。如index.html中的相关内容，\_post文件夹下的相关内容，img文件夹下相关内容等。

#### 要点3：之后

之后博客就算是正式建好了，然后需要做的事情还有：

**1** 熟悉Jekyll文件组织

**2** 熟悉Markdown语法

**3** 坚持不懈的写下去



## 其他

Jekyll是一款很火的开源静态网站建站工具，拥有社区、庞大用户群（意味着你能轻易找到解决问题的答案），各种插件、主题，无数的轮子。

Jekyll主要配置文件为根目录下的_config.yml文件

Jekyll对于博文，都是要求放在_posts目录下面，同时对博文的文件名有严格的规定，必须保持格式YEAR-MONTH-DAY-title.MARKUP，通常情况下，采用推荐的Markdown撰写博文。

写好的博文可在本地预览，但是要安装Ruby，Gem，Jekyll，略麻烦。

绑定域名，也很麻烦，主要的麻烦是在国内网站需要备案。

图床，可以使用github，但是不好迁移。考虑到以后迁移，可以使用sm.ms。

#### Jekyll组织结构

一个标准的使用Jekyll工具生成的网站,其目录结构一般是像这样的:

![Jekyll组织结构](https://i.loli.net/2018/04/05/5ac605b66b783.png)

简单介绍一下每个目录和文件的作用：

![文件目录结构](https://i.loli.net/2018/04/05/5ac605fc0a5be.png)



















