---
layout:     post
title:      Tensorflow GPU版本极简安装教程
subtitle:   人生苦短，我用conda
date:       2020-12-7
author:     WastedYears
header-img: img/post-bg-2015.jpg
catalog: 	 true
tags:
    - 原创
    - 教程
    - 深度学习
    - python
---

>  给还拎不清的小组员写的亲妈级教程

## 1.安装任意版本anaconda

理论如此 但最好不要追新 推荐[Anaconda3-2020.02-Windows-x86_64.exe](https://repo.anaconda.com/archive/Anaconda3-2020.02-Windows-x86_64.exe)

点击即可下载

如果已经安装了不用重装 直接跳步

## 2.先运行anaconda一次

第一次打开会自动为你安装jupyter notebook等程序   速度较慢  成功打开后关闭

## 3.运行anaconda prompt

![2020-12-07.png](https://i.loli.net/2020/12/07/BGRxltKUZEW4Le3.png)

点击第三排那个

### 1.输入

```
conda create --name tensorflow python==3.7
```

回车

![输入]( https://i.loli.net/2020/12/07/2lfBKCopwODWSAe.png)

输入 y

安装成功后显示

![QQ截图20201207163210.png](https://i.loli.net/2020/12/07/aMWE9nO3vLimuzj.png)

### 2.输入

```
activate tensorflow1
```

回车

安装成功后显示

![QQ截图20201207163210.png](https://i.loli.net/2020/12/07/7OQq4pvnAJc5LVE.png)

### 3.输入

``` 
conda install tensorflow-gpu==2.0
```

![QQ截图20201207163210.png](https://i.loli.net/2020/12/07/JG46QUtZ7evLqfK.png)

回车

注意看此处是否是你需要的版本

![QQ截图20201207163210.png](https://i.loli.net/2020/12/07/nMY46oPHueU9qQw.png)

输入y开始安装

![QQ截图20201207163210.png](https://i.loli.net/2020/12/07/GmA92SBtzh7JQNC.png)

此时不要乱点  点到cmd里容易暂停  暂停时间久了就会自动断开  导致安装不成功 我第一次就是这样导致CUDA没装上

若还是安装失败了 重复此步骤  conda会自动检测修复  不会重复安装的

![QQ截图20201207163210.png](https://i.loli.net/2020/12/07/6lR5KOrxgTB1tkV.png)

成功

### 4.输入

```
conda install keras==2.3.1
```

![QQ截图20201207163210.png](https://i.loli.net/2020/12/07/kxP9hzWMygDsUGm.png)

成功

### 5.输入

```
conda install nb_conda
```

回车

打开jupyte notebook

可见

![QQ截图20201207163210.png](https://i.loli.net/2020/12/07/68s2IbBYZPgdCre.png)

此环境已加入

# 全文完  感谢阅读

## ps：

后面训练书上5.2模型会用到pillow包 顺手一起安装了

输入 

```
pip install pillow
```

 注意，此处安装不要在虚拟环境中安装 请一定回退到base

成功安装显示如下

![QQ截图20201207163210.png](https://i.loli.net/2020/12/07/H3pW72DmaPyIN9O.png)

