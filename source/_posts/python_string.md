---
title: 'python字符串'
date: 2021-01-08 12:39:39
tags: python
category: Code
---

##### 字符串常用操作
* `s.count(s1)`
计算字符串s1在s中出现的次数。
* `s.find(s1)`
返回子字符串s1在s中第一次出现的索引值，如果s1不在s中，则返回-1。
* `s.rfind(s1)`
功能与find相同，只是从s的末尾开始反向搜索。
* `s.index(s1)`
功能与find相同，只是如果s1不在s中，则抛出一个异常。
* `s.rindex(s1)`
功能与index相同，只是从s的末尾开始。
* `s.lower()`
将s中所有的大写字母转换为小写。
* `s.replace(old, new)`
将s中出现过的所有字符串old替换为字符串new。
* `s.rstrip()`
去掉s末尾的空白字符。
* `s.spilt(d)`
使用d作为分隔符拆分字符串s，返回s的一个子字符串列表。
