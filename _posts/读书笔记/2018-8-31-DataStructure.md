---
layout:     post
title:      读书笔记-数据结构与算法
category: 读书笔记
description: 读书笔记
tags: 算法
---

# 读书笔记-数据结构与算法分析

所谓数据结构就是 数据结构 + 算法两部分。知识点包括：
- 数据结构：包括数据的存储方式和操作接口，有数组、链表、栈和队列、树、Hash、优先队列（堆）等
- 算法：包括排序、搜索（DFS,BFS,二分，并查集）、动态规划、贪心、位运算、回溯、分治等；算法时间复杂度和空间复杂度

## 一、数据结构

### 1 链表

**关键点：**    插入删除快O(1)，查找慢O(n)<br>
**形式与应用:** 单链表、双链表、循环链表。内核等底层软件中都有链表作为基础数据结构。<br>
**操作:**       插入、删除、查找、合并等<br>

[练习题目](https://leetcode-cn.com/tag/linked-list/)

### 2 栈

**关键点：**    FILO <br>
**形式与应用:** 数组形式、链表形式。<br>
**操作:**       初始化，判空以及取栈顶元素<br>

[练习题目](https://leetcode-cn.com/tag/stack/)

### 3 队列

**关键点：**    FIFO <br>
**形式与应用:** 数组形式、链表形式。<br>
**操作:**       add、remove、element、offer、poll、peek、put、take<br>

[练习题目](https://leetcode-cn.com/tag/queue/)

### 4 树

**关键点：**    它是由 n(n>0) 个有限节点组成一个具有层次关系的集合，模拟树结构。<br>
**形式与应用:** 平衡树、RB树、二叉搜索树，应用有进程树。<br>
**操作:**       前、中、后序便利，查找<br>

[练习题目](https://leetcode-cn.com/tag/tree/)

### 5 哈希表

**关键点：**    查找快，键值对 <br>
**形式与应用:** 数组形式、链表形式，字符串哈希。<br>
**操作:**       初始化，get，set<br>

[练习题目](https://leetcode-cn.com/tag/hash-table/)

### 6 优先队列

**关键点：**    堆（Heap）是一个可以被看成近似完全二叉树的数组。树上的每一个结点对应数组的一个元素。除了最底层外，该树是完全充满的，而且是从左到右填充。—— 来自：《算法导论》

堆包括最大堆和最小堆 <br>

**形式与应用:**  数组形式，网络收发<br>
**操作:**       插入，获取，平衡<br>

[练习题目](https://leetcode-cn.com/tag/heap/)

## 二、算法

### 1 排序
### 2 搜索
### 3 DFS
### 4 BFS

### 5 二分
[详解](https://www.baidu.com/link?url=2fX4orYaloK_FWx9R6iuQBRdD6QtkaXxDqLhr9Mcy97nMr17MQTIgGGx4C6Ze0Ml9BHP7In7zvKWSPCwefm36_&wd=&eqid=e9d4323a000b7d24000000045e47dd4e)

**注意点：**
- while 循环的条件中是 <=
- 包括所有搜索条件

### 5 并查集
### 6 动态规划
[详解]

**注意点**
- 拆解子问题，通过子问题求解问题
- 动态规划常常适用于有重叠子问题和最优子结构性质的问题
- 具有天然剪枝的功能，从而减少计算量：一旦某个给定子问题的解已经算出，则将其记忆化存储，以便下次需要同一个子问题解之时直接查表。

### 7 贪心
### 8 位运算

### 9 回溯
**注意点**
怎么遍历不同场景的路径很关键，知道了怎么遍历就知道怎么用递归去构造，其次就是递归的传参，除了本身的参数，一般还有传递返回值参数、中间参数（stack），终止条件参数（eg.len）等

### 10 分治