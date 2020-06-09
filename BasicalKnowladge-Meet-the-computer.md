---
title: "初识计算机"
date: 2020-06-09T14:37:56+08:00
lastmod: 2020-06-09T15:37:56+08:00
draft: false
tags: ["计算机结构"]
categories: ["计算机基础知识"]
author: "Ipbase508-lhb"
contentCopyright: '<a rel="license noopener" href="https://en.wikipedia.org/wiki/Wikipedia:Text_of_Creative_Commons_Attribution-ShareAlike_3.0_Unported_License" target="_blank">Creative Commons Attribution-ShareAlike License</a>'
---

<!--上述为文章属性，请修改内容为“***”的部分、时间及版权声明
title 文章标题
tags标签，可填写一个或多个标签
categories分类根据实际内容请填写“计算机基础知识”、“实用技能”、“故障解决”中的一个
author作者仅填写第一作者，贡献者请在文末以Logo及链接的形式按照示例代码注明
推荐使用typora编辑器
-->

<!--文章内容最大标题等级为二级标题-->



## 计算机的硬件组成
让我们忘掉冯诺依曼原理，忘掉二进制，忘掉南桥北桥，忘掉各种计算机理论，只是单纯地看看我们面前这台计算机是怎样构成的。    

### 输入输出设备

相信在你面前，首先可以看到一块屏幕、键盘、还有鼠标，如果是笔记本电脑，加上机身这就是我们所有直观的认识，如果是台式电脑，再加上一个主机箱。   

分门别类是认识事物的好方法，我们不妨也这样开始我们的学习之旅。      

屏幕给我们显示和反馈信息，我们将其称之为输出设备，同理，扬声器、打印机等也可以称之为输出设备。

通过鼠标、键盘，我们向计算机传入信息，我们将其称之为输入设备，同理，手写板、摄像头、麦克风也可以归纳进输入设备。当然你的Xbox手柄也在其中。   

### 机箱内部组成

而剩下的我们还不了解的就是笔记本机身内部或者主机机箱内部的组成，笔记本内部结构其实和主机机箱内部没有根本的区别，通过组件的定制与编排，线路连接的改变等方式使得内部结构变得更为紧凑从而节省空间。所以为了更直观地认识计算机内部，我们不妨使用一个主机机箱内部进行介绍。   

实践能为我们我们的学习带来更为直观的体验，所以我们不妨动手组装一台台式机吧。Steam上的《装机模拟器》这款游戏能够为我们带来真实的装机体验，是的，装机也可以成为一款游戏。当然如果觉得过于麻烦，可以省略这一步，观看以下[视频](https://www.bilibili.com/video/BV1At411X7Wz)，从而了解台式计算机的内部组成。

![](http://47.107.149.229:8080/%E5%8F%B0%E5%BC%8F%E6%9C%BA%E6%9C%BA%E7%AE%B1%E7%BB%84%E6%88%90.PNG)

> ​														图片源自[视频](https://www.bilibili.com/video/BV1At411X7Wz)截图，侵权请联系删除

从上面的视频中可以看出，机箱内部的组成可以分为以下部分：机箱、电源、电源（连接）线、散热器、主板、CPU、内存条、硬盘、显卡（非必须）。    

那么这些部件的作用分别是什么呢？     

电源和电源线顾名思义负责供电；散热器负责散热；主板将各个部件连接在一起；CPU负责处理信息，运行程序；内存条，在以后的文章中，我们会将其称之为RAM，我们可以简单地将其理解为在硬盘将程序或信息送入CPU之前或者CPU将信息送出硬盘之前，RAM作为一个中间设备，缓存两者读写速度上的不匹配从而提高电脑的工作效率；硬盘，顾名思义负责存储信息，硬盘分为机械硬盘（HDD）、固态硬盘（SSD）以及一种比较少见的混合硬盘（HHD），笔者仅接触过一款三星的笔记本搭载了混合硬盘；显卡可以提高计算机处理图像的能力，这对于游戏爱好者，视频剪辑从业者十分重要。

### 小结

到这里我们将常见的计算机设备部件进行以下分类

| 设备类别 |              常见组件              |                                               作用 |
| :------: | :--------------------------------: | -------------------------------------------------: |
| 输入设备 | 键盘、鼠标、摄像头、麦克风、扫描仪 |                                   向计算机传送信息 |
| 输出设备 |       显示器、扬声器、打印机       |                                 计算机向外传送信息 |
| 处理单元 |                CPU                 |                                 处理信息、运行程序 |
| 中间设备 |                内存                | 提高计算机性能，缓存外部设备与处理单元速度的不匹配 |
| 外部设备 |                硬盘                |                                     存储程序与数据 |



## 计算机软件组成

### BIOS

传统的计算机软件系统可以简化为系统软件和应用软件。但在开始介绍软件系统前，我们有必要介绍一下BIOS。BIOS，Basic Input Output System，基本输入输出系统。    

BIOS作为计算机通电后执行的第一个程序，它并不存在于硬盘中，而是位于主板上的ROM或EPROM上。BIOS负责测试和初始化CPU、RAM、硬盘等设备。当所有的设备装载成功后，BIOS会尝试从硬盘、U盘、CD-ROM等可以存储操作系统的地方加载系统，这取决于BIOS中设置的启动顺序。

###  软件系统

我们将计算机软件系统分为系统软件和应用软件。系统软件包括操作系统、数据库系统、语言处理系统等，当然我们最熟悉的就是软件系统。应用软件则是我们日常使用到的软件，这些软件依赖于操作系统运行。本站的大部分内容也都是围绕操作系统展开的，后续我们将会增加关于操作系统使用和维护方面的文章。



## 参与本项目

[GitHub](https://github.com/LHB6540/windows-computer-maintenance-guide) 

## 交流学习

广中医电脑义修咨询群：465636714

Windows使用与日常维护交流Ⅱ群：982188851



## 贡献者

<center class="half">
  <a href="https://github.com/lhb6540">
    <img src="https://avatars3.githubusercontent.com/u/41095303?s=460&v=4" width="30"/>
  </a>
</center>

