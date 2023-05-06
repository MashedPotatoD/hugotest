---
title: "Fisrt Md"
date: 2023-05-04T17:14:56+08:00
draft: false
---
[TOC]


# 这是我写的第一份md文档,用于学习markdarn语法

## 1.第一部分测试代码块
``` golang
import(
    "fmt",
)
fmt.Println("hello呀")
```
这是行内代码`fmt.Println("hello呀")`

## 2.第二部分测试列表
### 2.1首先是有序列表
1. 第一
2. 第二
    1. 第二个的第一个
    2. 第二个上的第二个

### 2.2然后是无序列表
- 一级
    - 二级
    - 二级
      - 三级

## 3.第三部分测试倾斜,加粗和删除线
*这是倾斜*
**这是加粗**
***这是倾斜+加粗***
~~这是删除~~

## 4.第四部分测试表格
左对齐 | 居中 | 居中 | 右对齐
:-- | :--: | :--: | --:
1|2|3|4
5|6|7|8

## 5.第五部分测试插入图片
### 5.1测试本地图片
![本地图片](./hero.png?raw=true&cachebuster=1)
尝试了给图片地址前加上./
也尝试了将图片的名字简化
但是都没有奏效,依然无法在个人博客中显示出来

### 5.2测试网络图片
![网络图片](https://images.pexels.com/photos/14454925/pexels-photo-14454925.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load)
网络图片可以正常显示

## 6.第六部分测试插入链接
[这是一个百度的链接](http://baidu.com)

## 7.第七部分测试表情
:smile:
:heart:
:wink:
:thumbsup:
:thumbsdown:
成功啦~:wink:

## 8.第八部分测试给文字变色
<span style="color:cyan;">这段文字会变成青色</span>

## 9.第九部分测试强制换行
听说要两个空格和一个回车  
成功了耶~