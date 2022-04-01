---
title: 【算法-简单】斐波那契数 
author: RemMai
avatar: 'https://cdn.jsdelivr.net/gh/remmai/cdn@1.0/img/custom/avatar.jpg' 
authorLink: 'https://blog.RemMai.cn'
authorAbout: 一个不怎么幸运的男孩~
authorDesc: 一个不怎么幸运的男孩~
comments: true
date: 2020-05-15 01:02:40
tags: [算法,面试]
keywords:
description:
photos: 
    - http://p2.qhimg.com/bdr/__100/t01b079bc5131c99a6b.jpg
---
# [算法-简单]斐波那契数 

> 0,1,1,2,3,5,8,13,21......找规律。  

## 方法一：递归
> 非最优解，耗时。【百度即可得到答案】

## 方法二；动态规划
> 个人认为的最优解。
```python
def fib(i):
    dp_0, dp_1 = 0,1
    for _ in range(i):
        dp_0, dp_1 = dp_1, dp_0 + dp_1
    return dp_0
```

# 总结
递归的耗时远超过动态规划，0-30的话，完全可以通过查表法。