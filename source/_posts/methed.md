---
title: html dom
date: 2016-08-09 14:30:46
tags:
---
***
## html dom
### 一些常用的dom方法
* getElementById(id)-获取带有指定id的节点(元素)
* getElementsByTagName()-获取包含带有指定标签名称的所有元素的节点列表(集合/节点数组)
* getElementsByClassName()-获取包含带有指定类名的所有元素的节点列表
* appendChild()-把新的子节点添加到指定节点
* removeChild()-删除子节点
* replaceChild()-替换子节点
* insertBefore()-在指定的子节点前面插入新的子节点
* createAttribute()-创建属性节点
* createElement()-创建元素节点
* createTextNode()-创建元素节点
* getAttribute()-获取指定的属性值
* setAttribute()-把指定属性设置或修改为指定的值
* appendChild(node)-插入新的子节点(元素)
* removwChild(node)-删除子节点(元素)

### 一些常用的dom属性
* innerHTML-节点(元素)的文本值
* parentNode-节点(元素)的父节点
* childNodes- 节点(元素)的子节点
* attributes -节点(元素)的属性节点

### node属性
nodeName属性规定节点的名称，具有以下特点
* nodeName是只读的
* 元素节点的nodeName与标签名相同(不区分大小写)
* 属性节点的nodeName与属性名相同
* 文本节点的nodeName始终是#text
* 文档节点的nodeName始终是#document

nodevalue属性规定节点的值，具有以下特点
* 元素节点的nodeValue是undefined 或 null
* 文本节点的nodeValue是文本本身
* 属性节点的nodeValue是属性值
nodeType属性返回节点的类型，是只读的，比较重要的节点有
元素类型				nodeType
元素					1
属性					2
文本					3
注释					8
文档					9





**Author：lgcsser**