---
title: "关于"
date: 2020-06-08T21:38:52+08:00
lastmod: 2020-06-08T21:41:52+08:00
menu: "main"
weight: 50

---

## 项目说明   
本项目由广州中医药大学学生创新实践基地运维部维护和管理。网站初始内容源自运维部义修培训指南,出于隐私等目的，移除了培训指南中的内部规范和章程的部分。

运维部除了面向成员提供运维知识学习外，同时也面向学校师生提供计算机义修服务。在大多数情况下，我们处理的工单是安装了Windows操作系统的个人电脑，
义修的过程也是一个学习的过程，在遇到问题时，我们也会去网上查阅资料。但我们发现资料过于分散，甚至难以找到一个活跃度高、专业性强的关于Windows
维护的网站，于是萌生了搭建一个平台，系统地分享windows计算机维护经验的平台的想法。   

为什么使用GitHub和静态网页？或许使用一个类似WordPress的交互式博客或者BBS系统可以更充分地互动和交流，但这同时也会增加内容管理、筛选的服务成本和服务器运行的成本，笔者暂时没有这个精力和资源。GitHub作为一个知名的代码协作平台，借助着用户的专业性和社会化编程的共享精神，相信项目内容会很快得到优质的补充，同时，这或许会让找程序员修电脑不再成为一个梗😂。借助GitHub Actions，将内容继续更新到网页，方便大众能够方便的获取所需的知识。

## 内容组成
本指南分为三种类型的内容：计算机基础认识、基础维护技能和故障修复       
其对应的GitHub仓库文件为BasicKnowledge-{}.md，Skills-{}.md，Issues-{}.md,其中{}中的为内容的摘要的英文名称。如果摘要内容重复，添加-{数字} 以区别      

## 如何加入本项目为本项目做贡献
### 一、本项目内容使用两种方法呈现：   
GitHub仓库的Markdown文件    
基于Markdown文件借助Hugo生成的静态网页。本项目将借助GitHub Actions进行CI/CD   

### 二、我们期望的所贡献的内容包括但不限于以下内容：   
1、对于项目已有内容的错误之处的勘正     
2、对于项目已有内容的合理拓展
3、新的经验 或知识分享
4、将您在计算机维护过程中遇到的新问题及解决过程与思路向仓库添加一篇分类为”故障修复“，文件命名为Issues-{}的md文档    
5、将您在计算机维护过程中遇到的未解决的新问题发布到Issues中，我们将进行解答并根据情况添加一篇分类为“故障修复”文档   

### 三、如何加入本项目为本项目做贡献：
- 第一次进行贡献：  
  1、将本仓库fork至您的GitHub仓库，您需要提前拥有有个GitHub账户   
  2、在Git Bash中克隆您的仓库，请注意区分原仓库和您的仓库

  ```bash
  git clone https://github.com/[your name]/windows-computer-maintenance-guide-Programmers-also-repair-Win-PC.git
  ```

  3、对于新发布的文章，进入您的计算机中的仓库，复制templete.md至content/post目录中。根据上述内容组成中的命名规则命名文章。编辑文件，根据文件中的提示，修改文件开头的文章属性。删除提示内容，编辑您的文章。

  ​	  对于已有文章的勘误、补充等修改行为，根据原网页链接中最后一个/后面的字符在content/post中找到对应的文件，然后开始您的修改。

  ​	 在贡献后，请不要忘记在文末添加您的贡献编辑，它由有一个icon和个人主页链接组成。

  4、提交你在本地计算机的更改到您的GitHub仓库

  ```bash
  git add * 
  git commit -m '简单描述您的更改'
  git push
  ```

  5、在GitHub中发起pull request到本项目的仓库。如果您在pull request收到目标仓库已更改的警告，请参考下方的第n次贡献。
  
- 第n次贡献：

  如果项目足够活跃，在您发起pull request的时候，可能会遇到目标仓库已更改的警告。这意味着您的仓库与原仓库的版本不一致，你需要将您fork的仓库与源仓库保持同步更新已解决问题。当然您也可以直接删除fork的仓库，再次fork最新的仓库，这是不建议的，因为会丢失您的更改记录(如果您在意这些历史更改)

  1、进入您在本地计算机的仓库，检查远程仓库路径

  ```bash
  git remote -v
  ```

  2、如果您只看到两行orgin开头的文本，并且后跟的链接为您的仓库，则您需要将本项目的远程仓库设置为您的上游仓库

  ```bash
  git remote add upstream https://github.com/LHB6540/windows-computer-maintenance-guide-Programmers-also-repair-Win-PC.git
  #再次输入git remote -v以检查是否添加成功
  ```

  3、将本地的更改推送到您的远程仓库

  ```bash
  git add
  git commit
  git push
  ```

  4、拉取本仓库的更新

  ```bash
  git fetch upstream
  ```

  5、合并分支并推送至远程仓库

  ```bash
  git checkout master
  git merge upstream/master
  git push
  ```

  6、发起pull request
## 感谢您的贡献
我们期待您加入本项目并为本项目做出贡献。
