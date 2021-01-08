---
title: 'python序列'
date: 2021-01-08 12:39:39
tags: python
category: Code
---

##### python序列
* tuple: 元组是一些元素的不可变有序序列
`(1, 'two', 3)`

* range: 范围不可变
`range(start, stop, step)`

* 列表: 值的有序序列，可变
`['I did it', 4, 'all']`  
<!-- more -->
##### 序列str, tuple, range, list通用操作
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