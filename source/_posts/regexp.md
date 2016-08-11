---
title: Javascript regexp正则对象
date: 2016-08-08 14:32:40
tags: regexp
---
***
## 新建正则对象
新建正则
* 字面量 var regexp = /xyz/;编译时新建,推荐使用该方法
* 使用regexp函数，var regexp = new RegExp('xyz');在运行时新建，不推荐使用该方法。

正则对象生成后，有2种使用方法：
#### 属性
* 正则对象的方法，将字符串作为参数，比如regexp.test(string)
* 字符串对象的方法,将正则对象作为参数，比如string.match(regexp)

## 正则对象的属性和方法
正则对象的属性分为2类
* 修饰祥光的，返回一个布尔值，表示相应的修饰符是否设置。
```
1.ignoreCase：表示是否设置了i修饰符
2.global：表示是否设置了G修饰符
3.multiline：表示是否这是了m修饰符，
```
* 与修饰无关
```
lastIdex：返回下一次开始搜索的位置，该属性可读写，但是只在设置了g修饰符时有意义
source：返回正则表达式的字符串形式（不包括反斜杠），该属性只读
```
#### test()该方法返回一个布尔值，表示当前模式是否能匹配参数字符串
```
var r = /'cat'/;
r.test('cat and dog'); //ture
```
上面代码验证参数字符串之中是否包含cat，结果为true；
如果正则表达式带有g修饰符，则每一次test方法都从上一次结束的位置开始向后匹配。
```
var r = /x/g;
var s = '_x_x';
```


## 字符串对象的属性和方法

**Author：lgcsser**