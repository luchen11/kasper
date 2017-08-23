---
layout: post
title:  "linux下安装Clion与Idea"
date:   2017-08-18 01:01:00
categories: essay
---

## JetBranins<b>
JetBrains是一家捷克的软件开发公司，该公司位于捷克的布拉格。
Clion和Idea就是该公司出品的软件，该家公司的软件以精品著称。所有的软件都可以到[官网](https://www.jetbrains.com) 上进行下载。

## Clion和Idea
在Linux下用于进行c++开发的集成环境很少，很多都是使用文本编辑器和编辑器进行开发。开发的速度相对来说有待提高。
codeblock 在做大的项目上，有很多的功能不够完善，Clion的出现解决了这些问题。但是，Clion毕竟是一个新的软件，还有很多的地方需要进一步的完善。
例如:
 ** 1 不能够选择编译器，Clion自动到/usr/bin/下寻找gcc/g++,不能指定特定的编译器，比如clang。
** 2 编译器不能够添加编译选项，选项的内容可以在cmake文件中添加。可能这是一个功能，而不是bug。

linux下java的IDE以前也有，比较著名的Eclipse与MyEclipse。Idea不仅可以进行java的编写，也可以进行Android的开发。

## Clion的安装
直接[Clion下载](https://www.jetbrains.com/clion/) 进行下载，得到一个压缩包。一般命名为Clion-版本号.tar.gz

下载完成后就可以在终端进行解压。
` tar -xvf Clion-版本号.tar.gz `
将文件夹命名为clion
这是为了在设置路径的时候更简便一些。
将该文件夹复制到/opt下。
最后一步就是修改命令的路径。
在home目录下打开bashrc文件
` vi .bashrc `
在文件中添加一句
` export PATH=/opt/clion/bin:${PATH} `

至此，CLion的安装就完成了,现在就可以在启动器中找到Clion软件了。

Idea的安装也是一样的过程，借用一句数学语言--同理可得，这里不再叙述。

