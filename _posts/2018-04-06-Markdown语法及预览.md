---
layout:     post
title:      Markdown语法及预览
subtitle:	Markdown简要语法及在本地的预览
date:       2018-04-06
author:     Shaun
header-img: img/post-bg-github.jpeg
catalog: true
tags:
    - macbook
    - Markdown
---

## 起因

写博客需要，重新学一下Markdown语法。以及在MacBook上用Sublime写md时的预览方法。

# Markdown
Markdown是一种书写的格式，只涵盖纯文本可以涵盖的范围。

## 区块元素
* 段落和换行：前后要有一个以上的空行
* 标题：1-6个#，对应1到6级标题
* 区块引用：单行，大于号‘>’开头；可嵌套，根据不同层次嵌套不同的>
* 列表：用\*,\+,\-，三者是一样的，表示无序列表；有序列表为数字紧接一个.号。数字顺序问题；列表项目可包含多个段落；列表内可添加引用，需要缩进一次；若要放置代码块，则需缩进两次
* 代码块：缩进4个空格或1个制表符。
* 分割线：3个以上的\*号减号，底线等

## 区段元素
* 链接：以方括号和圆括号表示链接；圆括号内可在url后双引号加title；同主机内的资源可用相对路径;参考式链接，`[test][1]` , `[1]: https://...` link.；隐式链接，等同于链接文字，然后定义链接内容。 参考式链接的好处是，阅读感觉不被打断。
* 强调：一个\*或\_包围内容为斜体，两个为加粗，三个为斜体加粗；
* 代码：一个\`包围的内容
* 图片：行内式：`![Alt text](/path/to/img.jpg "Optional title")`;参考式：`![Alt text][id]`;目前为止，无法指定宽高

## 其他
* 自动链接：用于较短的自动链接或邮件，以尖括号包围
* 反斜杠：转义符号

# 在Sublime中的预览

## 插件安装
参考资料：[Sublime实时预览md插件](http://www.360doc.com/content/17/0827/11/13561030_682462772.shtml)

ctrl+shift+p，输入pcip到Package Control：Install Package，安装Markdown Editing和Markdown Preview

## md预览
ctrl+shift+p，输入mp到Markdown Preview:Preview in Browser
在md文件最下面一行添加：`<meta http-equiv="refresh" content="0.1">`.(实测不好用)，要实时预览可用其他方式。

# 其他
## 各种app
[马克飞象](https://maxiang.io/)：本地版，网页版，chrome app版。是最开始用的。收费版可关联印象笔记。

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522949518172&di=11e3dfdddc70f72beb30f8dad0ca1f61&imgtype=0&src=http%3A%2F%2Feasyread.ph.126.net%2Flq2cJjOgxiBi5dlemfaJhg%3D%3D%2F7916703622314805815.jpg)

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522949483069&di=a2651b99c5562ce95ec7c46a89078f9c&imgtype=0&src=http%3A%2F%2Fimg.kuqin.com%2Fupimg%2Fallimg%2F141112%2F2052114611-3.png)

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522949486336&di=2157c5dfaa9ae68d2456cc48cb5df0ab&imgtype=0&src=http%3A%2F%2Fimage.codes51.com%2FArticle%2Fimage%2F20160319%2F20160319082356_6389.png)

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522949522020&di=889a1cfa7f4990573731a58703d3a84d&imgtype=0&src=http%3A%2F%2Faliyunzixunbucket.oss-cn-beijing.aliyuncs.com%2Fjpg%2F0bf0d8946c7130b2919c86d6759e7bbd.jpg%3Fx-oss-process%3Dimage%2Fresize%2Cp_100%2Fauto-orient%2C1%2Fquality%2Cq_90%2Fformat%2Cjpg%2Fwatermark%2Cimage_eXVuY2VzaGk%3D%2Ct_100)

******

[Typora](https://typora.io/) ：所见即所得，实时预览的LaTeX公式，要在 Typora 里显示源码，可以用 command + / 切换。Typora在搭配iPic上传图片去图床是非常非常好用的。非常好用，最后选用的。

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522949664369&di=ebe01d7a68749d7722073de982fced7e&imgtype=0&src=http%3A%2F%2Fimg.smzy.com%2Fimges%2F2017%2F0622%2F20170622092419560.jpg)

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522949662365&di=8496132ca92ccbb0b0b9dd17e62d0b20&imgtype=0&src=http%3A%2F%2Fimg.zcool.cn%2Fcommunity%2F02785357911ed60000012e7e4762a3.jpg)

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522949664105&di=6009aa01da0f18b526c362e27e7213e6&imgtype=0&src=http%3A%2F%2Fww2.sinaimg.cn%2Flarge%2F97ded95egw1f7zacoxfhfj21hc0sm0wm.jpg)

******

[Mou](http://25.io/mou/)：在线预览，简洁；对代码支持不好；

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522949812715&di=c6cc8bf2ea899a5c7edcbb20dc0f5dee&imgtype=0&src=http%3A%2F%2Fmac.quweiwu.com%2Fuploads%2Fscreenshots%2Fmac_20121108144840_ba873799b2.png)

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522949850456&di=3c08dac78c2f266a62cdc686692233a9&imgtype=0&src=http%3A%2F%2Fimages2015.cnblogs.com%2Fblog%2F764197%2F201601%2F764197-20160126160101551-1933461185.png)

******

[Ulysses III](https://ulyssesapp.com/) ：界面好看，多级文件管理和iCloud云同步，多种格式导出，灵活标记语言定制；贵，不是所见即所得，没有数学公式

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522984295883&di=3753a3cb2430cf857a6d48f2bcac9b5b&imgtype=0&src=http%3A%2F%2Fwww.pc6.com%2Fup%2F2014-5%2F13994410948801222.jpg)

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522984291689&di=75e3f19d831e6c7fa8436005d68d230e&imgtype=0&src=http%3A%2F%2Fwww.cncrk.com%2Fup%2F1503%2F201503171301568468.jpg)

******

[haroopad](http://pad.haroopress.com/)：显示效果不错，支持代码高亮，支持vim快捷键；无法导出pdf

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522984494795&di=3c49b4dca81db28af9af5be56f517517&imgtype=jpg&src=http%3A%2F%2Fimg3.imgtn.bdimg.com%2Fit%2Fu%3D4288014583%2C1299116437%26fm%3D214%26gp%3D0.jpg)

******

[Atom](https://atom.io/)：github出的一款编辑器，插件强大，主题丰富；不支持在线预览（现在好像支持了）

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522984657156&di=79a1bc07e4142db8f1ca0922ff53cec6&imgtype=jpg&src=http%3A%2F%2Fimg2.imgtn.bdimg.com%2Fit%2Fu%3D2470201542%2C2653351995%26fm%3D214%26gp%3D0.jpg)

******

[Sublime](https://www.sublimetext.com/)：同Atom，插件超多。目前是使用网页预览，略慢。

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522984733855&di=0598b9636dbd2406f842f16ba525bfa6&imgtype=0&src=http%3A%2F%2Fimages0.cnblogs.com%2Fblog2015%2F763969%2F201506%2F141310043946500.png)

******

[stackedit](https://stackedit.io/)

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522984844539&di=a82f142bdd9ee019fbad61a0fb748210&imgtype=0&src=http%3A%2F%2Fstatic.open-open.com%2Fnews%2FuploadImg%2F20150321%2F20150321180401_418.png)

******

[TextNut](http://www.textnutwriter.com/)

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522984869580&di=eec026de6005052564772ce6f3605652&imgtype=0&src=http%3A%2F%2Fpic.orsoon.com%2Fuploads%2Fallimg%2F62841453452020.jpg)

******

[marktext](https://github.com/marktext/marktext)可实时预览
![](https://dn-cnode.qbox.me/FvWhG1Ke30sJZ7kUf9QzERBcSCDm)

******

[Quiver](http://happenapps.com/#quiver)
![](https://pix.waerfa.com/2015/12/Quiver%20four%20cells.png)

******

[MacDown](http://macdown.uranusjr.com/)：简洁美观，代码高亮，自定义主题，导出pdf
![](http://macdown.uranusjr.com/static/images/macdown-demo.png)

******

[Marboo](http://marboo.io/)：简洁优美，支持笔记本的形式管理；只是个外壳，需要调第三方软件
![](http://medis.qiniudn.com/1.jpg)

******

[gitbook](https://legacy.gitbook.com/)，很多人用来写书

![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1522985215931&di=79e93e1681757f3258902f8c168b32ae&imgtype=0&src=http%3A%2F%2Fi-3.yxdown.com%2F2015%2F12%2F30%2Fb66107b8-c76e-4dc4-92f8-4d5965d37993.png)

******

[Bear](http://www.bear-writer.com/) 颜值高，功能强大

![](https://pix.waerfa.com/Bear%20demo%201.gif)

******

其他还有很多，比如leanote,mdeditor,Marxico,Byword,Dayone,VS Code,MWeb,TextMate 2,简书,emacs,Docbook,Markdown Extra,MultiMarkdown, Maruku等，有些是专门写Markdown的，有些只是顺带支持Markdown。其中leanote是个开源软件，类似于印象笔记，主要是做笔记的。Dayone主要是用来写日记的，也很好用。VS Code类似于Sumlime text，就是个编辑器，要安装插件才能支持Markdown。简书是个在线的博客网站，支持Markdown的写法。emacs，神之编辑器，对新手不友好，且主要也不是用来写Markdown的。

总而言之，言而总之，以上应用使用起来大同小异，根据自己需要选择在线或者本地版，作为一个工具，只要使用的人用得顺手就好。

进阶的玩法还有各种代码高亮，缩进，排版，LaTex，公式，表格等等等等，以及各家不一的增强语法，精力有限，不一一赘述。


#### 参考

[Markdown语法说明](https://www.appinn.com/markdown/)











