---
description: limit
---

# 查询第n高的数据

如果问题是找某组数据中，第n高的数据，多次子查询就会变得非常麻烦  
所以考虑使用limit用法

* limit y：读取y条数据
* limit x, y：跳过x条数据，读取y条数据
* limit y offset x：跳过x条数据，读取y条数据

#### 举例：

test1

| id | number |
| :--- | :--- |
| 1 | 100 |
| 2 | 200 |
| 3 | 300 |

test2

| secondhighestnumber |
| :--- |
| 200 |

例如上述的test1表，查询第2高的number，如果不存在第二高的number，查询返回null

`select ifnull(  
    (select distinct number from test1 order by number desc limit 1, 1), null  
) as test2;`

distinct 是去重操作

ifnull 判断空值的函数

* ifnull\(a,b\)
* 如果value1不为空，结果返回a
* 如果value1为空，结果返回b

