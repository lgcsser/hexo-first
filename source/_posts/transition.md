---
title: CSS3之-Transition过渡
date: 2016-06-06 10:50:39
tags:
---
***
# Transition过度
通过css3，我们可以再不使用flash动画或者JavaScript脚本的情况下，当元素从一种样式变换为另一种样式时，为元素添加效果。
要实现这一点，必须规定两项内容：
* 规定您希望把效果添加到那个css属性上
* 规定效果的时长


### 属性
* transition 简写属性，用于在一个属性中设置四个过度属性
* transition priperty 规定应用过度属性的css属性的名称。默认是all，所有属性都将获得过渡效果。none：没有属性会获得过渡效果，property：定义应用过渡效果的css属性名称列表，列表以逗号分隔
* transition duration 定义过度效果花费的时间。默认是0
* transition timing function 规定过度效果的时间曲线。默认是ease
* transition delay 规定过度效果何时开始。默认是0

时间曲线函数：
linear 匀速（等于 cubic-bezier(0,0,1,1)）
ease 慢速开始，然后加速，然后慢速结束（cubic-bezier(0.25,0.1,0.25,1)）
ease-in 慢速开始 （等于 cubic-bezier(0.42,0,1,1)）
ease-out慢速结束 （等于 cubic-bezier(0,0,0.58,1)）
ease-in-out 慢速开始和慢速结束 （等于 cubic-bezier(0.42,0,0.58,1)）
cubic-bezier(n,n,n,n)自定义，取值为0到1之间的数值。

**Author：lgcsser**