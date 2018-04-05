---
layout:     post
title:      Macbook更新git账号
subtitle:	MacBook SSH KEY免密远程登录github
date:       2018-04-05
author:     Shaun
header-img: img/post-bg-github.jpeg
catalog: true
tags:
    - macbook
    - github
---

因为觉得之前的github账号用户名太长不好看，于是重新申请了一个。于是本地的git崩了，需要重新配置一下。方法如下：

#### 1.重新生成SSH KEY:

>ssh-keygen -t rsa -C yzr@2064@gmail.com

>git config --global user.name zryang
>git config --global user.email yzr2064@gmail.com

#### 2.查看.pub文件：

cat ~/.ssh/id_rsa.pub
有以ssh-rsa开头的字符串

#### 3.将key添加到github中：

头像，Settings，SSH and GPG keys，New SSH Key

#### 4.删除本地钥匙串中的全部和git有关的内容。输入两次

>ssh -T git@github.com
会得到：
>GitHub does not provide shell access.

#### 5.clone下github中的一个库，然后添加文件，add，commit，push。

此时会需要填写github的username和Password，填写新的github用户名和密码即可。