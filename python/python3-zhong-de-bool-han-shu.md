---
description: bool() 函数输出的一些说明
---

# Python3 中的 bool\(\) 函数

## bool\(\[x\]\)

### 作用：

讲 x 转换为 Boolean 类型，如果 x 缺省，返回 False，bool 也为 int 的子类

### 参数 x :

任意对象或缺省；

> 注意：这里使用了\[x\]，说明x参数是可有可无的，如果不给任何参数则会返回False。

### 说明：

* 如果参与算数运算的话，True 相当于 1，False 相当于 0
* 将 x 转换为 bool，其本质是根据一定的规则返回内建的 True 或者 False 对象 规则：
  * 1. None 为 False
    2. 数字类型（int, float......），0 为 False，其他为 True
    3. 列表类型（list, tuple......），长度为 0 的为 False，其他为 True
    4. 字符串类型（str），长度为 0 的为 False，其他为 True
    5. 字典类型（dict），条目个数为 0 的为 False，其他为 True
    6. 任何其他类型的对象均为 True

