layout: port
title: 定时器
date: 2016-06-30 16:50:37
tags:
---
***
## js中提供定时执行代码的功能，叫做定时器，主要是setTimeout()&&setInterval()这两个函数完成。
* setTimeout()用于指定某个函数或者代码段，在一定时间之后执行，它返回一个整数，表示定时器的编号，以后可以用来取消该定时器。
语法如下：
```
var timeId = setTimeout(function | code, delay)
```
setTimeout函数接收2个参数，第一个参数function or code 是将要推迟执行的函数名字或者一段代码，第二个参数delay是推迟执行的毫秒数。
```
console.log(1);
setTimeout('console.log"2"',1000);//1000毫秒是1秒
console.log('3')
```
结果是1,3,2因为setTimeout指定第二条语句延迟1s执行。