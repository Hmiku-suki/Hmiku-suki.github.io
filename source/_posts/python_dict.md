---
title: 'python字典'
date: 2021-01-08 12:39:39
tags: python
category: Code
---

##### 字典
字典类型的对象与列表很相似，但字典使用键对其中的值进行引用，可以将字典看作一个键/值对的集合。
`dict = { key1:value1, key2:value2, key3:value3}`

字典中的项目是无序的，不能通过索引引用。
字典是可变的，可以添加或改变其中的项目。

<!-- more -->

##### 字典常用操作
* `len(d)`
返回d中项目的数量。
* `d.keys()`
返回d中所有键的视图。
* `d.values()`
返回d中所有值的视图。
* `k in d`
如果k在d中，则返回True。
* `d[k]`
返回d中键为k的项目。
* `d.get(k, v)`
如果k在d中，则返回d[k]，否则返回v。
* `d[k] = v`
在d中将值v与键k关联。如果已经有一个与k关联的值，则替换。
* `del d[k]`
从d中删除键k。
* `for k in d`
遍历d中的键。

