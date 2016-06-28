---
title: jQuery中this与$(this)的用法区别
date: 2016-06-28 11:52:05
tags:
---
***
## jQuery中this与$(this)的用法区别
```
$("#textbox").hover(function() {
  this.title = "Test"; 
}, 
fucntion() { 
  this.title = "OK”; 
}); 
```
 这里的this其实是一个Html 元素(textbox)，textbox有text属性，所以这样写是完全没有什么问题的。 但是如果将this换成$(this)就不是那回事了，就会报错了。 以下写法是错误的：
``` 
$("#textbox").hover( function() {
  $(this).title ＝ "Test"; 
}, 
function() { 
  $(this).title = "OK"; 
});
```
这里的$(this)是一个JQuery对象，而jQuery对象沒有title 属性，因此这样写是错误的。 JQuery拥有attr()方法可以get/set DOM对象的属性，所以正确的写法应该是这样： 正确的写法:
```
$("#textbox").hover( function() { 
  $(this).attr('title', 'Test'); 
}, 
function() { 
  $(this).attr('title', 'OK'); 
});
```
使用JQuery的好处是它包裝了各种浏览器版本对DOM对象的操作，因此统一使用$(this)而不再用this应该是比较不错的选择。