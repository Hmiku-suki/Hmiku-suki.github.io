---
title: 'nowcoder练习'
date: 2021-02-22 12:39:39
tags: python
category: Code
---

此篇记录了在nowcoder代码练习的一些东西。

<!-- more -->
#### NC78 反转列表
```python
# -*- coding:utf-8 -*-
# class ListNode:
#     def __init__(self, x):
#         self.val = x
#         self.next = None
class Solution:
    # 返回ListNode
    def ReverseList(self, pHead):
        # write code here
        if not pHead:
            return None
        newpHead = None
        while pHead:
            pHead.next, newpHead, pHead = newpHead, pHead, pHead.next
        return newpHead
```
令后一个结点指向前一个结点，并且将表头指针指向最后一个结点即可。  
