---
description: 一些写sql和出sql题目的规范
---

# Standard for Sql

## 字段名称

1. 全部小写
2. 使用全写，蛇形命名

例：

StuId \(False\) ------------------------------------ student\_id \(True\)

## 题目所需交付

* 数据（每题10组，8组测准确，2组测效率）
* 代码（standard）
* 错法列表 ------- 你能想到的可能出错方法，以及相应的错误代码

## 题目难度判定

* SQL 题难度定级 SOP： 
  * 入门\(Naive\): 只是用了一个语法的，比如 select \* from where , 最多用上 一个 join 或者 left join 
  * 简单\(Easy\): 用上两个语法知识进行组合的，或者 select 套 select 
  * 中等\(Medium\): 等我们出到更难的题目的时候再定这个标准
  * 难\(Hard\): 等我们出到更难的题目的时候再定这个标准

