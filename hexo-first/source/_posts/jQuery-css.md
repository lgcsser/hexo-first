---
title: jQuery-css
date: 2016-06-06 15:23:00
tags:
---
***
## jQuery css操作
* css() 设置或返回匹配元素的一个或多个样式属性。
* width() 设置或返回匹配元素的宽度
* height() 设置或返回匹配元素的高度
* offset() 返回第一个匹配元素相对于文档的位置
* offsetParent() 返回最近的定位祖先元素
* position()返回第一个匹配元素相对于父元素的位置
* scrollLeft() 设置或返回匹配元素相对于滚动条左侧的偏移量
* scrollTop() 设置或返回匹配元素相对于滚动条顶部的便宜量

### 一、css()

1. 获取css属性值
```
$(selector).css(name)
```
2. 设置单个语法
```
$(selector).css(property,value)
```
3. 设置多个语法
```
$(selector).css({property:value, property:value, ...})
```
4. 使用函数设置css属性
```
$(selector).css(property,function(index,value))
```
其中
- index - 可选。接受选择器的 index 位置
- oldvalue - 可选。接受 CSS 属性的当前值。

### 二、width()和height()

1.获取width or height.如果不为该方法设置参数，则返回以像素为单位的值
```
$(selector).width() or $(selector).height()
```
2.设置width() or height()
```
$(selector).width(length) or $(selector).height(length)
```
ps：length可选，如果没有规定长度单位则使用默认的px单位。

3.使用函数设置
```
$(selector).width(function(index,oldwidth)) or $(selector).height(function(index,oldheight))
```
其中
- index - 可选。接受选择器的 index 位置
- oldvalue - 可选。接受 CSS 属性的当前值。

** Author:lgcsser **