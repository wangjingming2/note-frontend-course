### WHERE后跟的是条件语句  
例：查询从a值到b之间的数据
```
SELECT * FROM 数据表 WHERE 字段1 >= a AND 字段1 <= b
```
或者
```
SELECT * FROM 数据表 WHERE 字段1 BETWEEN a AND b
```
例：查询叫王五的同学
```
SELECT * FROM 数据表 WHERE 字段1 = '王五'
```
或者
```
SELECT * FROM 数据表 WHERE 字段1 LIKE '王五'
```

例：查询姓王的同学。其中%是通配符
```
SELECT * FROM 数据表 WHERE 字段1 LIKE '王%'
```

例：查询名字中带“六”的同学
```
SELECT * FROM 数据表 WHERE 字段1 LIKE '%六%'
```

1. 跟在`-- `（含空格）之后的语句即是注释语句
2. `%六`表示以六结尾；`%六%`表示无论以什么开头，什么结尾只要包含“六”这个字；`六%`表示以“六”。
3. 关键字LIKE是一种模糊匹配；“=”是一种精确匹配

