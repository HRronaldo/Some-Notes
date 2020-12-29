---
description: limit
---

# 查询第n高的数据

如果问题是找某组数据中，第n高的数据，多次子查询就会变得非常麻烦  
所以考虑使用limit用法

* limit y：读取y条数据
* limit x, y：跳过x条数据，读取y条数据
* limit y offset x：跳过x条数据，读取y条数据

