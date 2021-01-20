---
title: 'python常见数据格式'
date: 2021-01-08 12:39:39
tags: python
category: Code
---

## python常见的一些数据格式及操作

<!-- more -->
#### python序列
* tuple: 元组是一些元素的不可变有序序列
`(1, 'two', 3)`

* range: 范围不可变
`range(start, stop, step)`

* 列表: 值的有序序列，可变
`['I did it', 4, 'all']`  
#### 序列str, tuple, range, list通用操作
* `seq[i]`
返回序列中的第i个元素。
* `len(seq)`
返回序列长度。
* `seq1 + seq2`
返回两个序列的连接(不适用于range)。
* `n*seq`
返回一个重复了n次的seq序列。
* `seq[start:end]`
返回序列的一个切片。
* `e in seq`
如果序列包含e，则返回True，否则返回False。
* `e not in seq`
如果序列不包含e，则返回True，否则返回False。
* `for e in seq`
遍历序列中的元素。  
#### 字符串常用操作
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
#### 列表常用操作
* `L.append(e)`
将对象e追加到L的末尾。
* `L.count(e)`
返回e在L中出现的次数。
* `L.insert(i, e)`
将对象e插入L中索引值为i的位置。<!-- more -->
* `L.extend(L1)`
将L1中的项目追加到L末尾。
* `L.remove(e)`
从L中删除第一个出现的e。
* `L.index(e)`
返回e第一次出现在L中的索引值。如果e不在L中，则抛出一个异常。
* `L.pop(i)`
删除并发返回L中索引值为i的项目。如果L为空，则抛出一个异常。如果i被省略，则i的默认值为-1，删除并返回L中的最后一个元素。
* `L.sort()`
升序排列L中的元素。
* `L.reserve()`
翻转L中的元素顺序。  
#### 字典
字典类型的对象与列表很相似，但字典使用键对其中的值进行引用，可以将字典看作一个键/值对的集合。
`dict = { key1:value1, key2:value2, key3:value3}`

字典中的项目是无序的，不能通过索引引用。
字典是可变的，可以添加或改变其中的项目。
#### 字典常用操作
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
#### 文件常用操作
`fn`为表示文件名的字符串  
`s`为字符串  
`S`为字符串序列  

* `open(fn, 'w')`
创建一个文件用来写入数据，返回文件句柄。
* `open(fn, 'r')`
打开一个已有文件读取数据，返回文件句柄。
* `open(fn, 'a')`
打开一个已有文件用来追加数据，返回文件句柄。
* `fh.read()`
返回一个字符串，其中包含与文件句柄fh相关的文件中的内容。
* `fh.readline()`
返回与文件句柄fh相关的文件中的下一行。
* `fh.readlines()`
返回一个列表，列表中的每个元素都是与文件句柄fh相关的文件中的一行。
* `fh.write(s)`
将字符串s写入与文件句柄fh相关的文件末尾。
* `fh.writeLines(S)`
将S中的每个元素作为一个单独的行写入与文件句柄fh相关的文件。
* `fh.close()`
关闭与文件句柄fh相关的文件。