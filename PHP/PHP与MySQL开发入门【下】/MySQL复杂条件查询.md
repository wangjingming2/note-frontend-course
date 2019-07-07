默认查询出来的数据是按照数据插入的时间排序的

关键字`ORDER BY`指定排序方式
例：按照字段名的值顺序排序
```
SELECT * FROM 数据表 ORDER BY 字段名
```
例：按照字段名的值逆序排序
```
SELECT * FROM 数据表 ORDER BY 字段名 DESC
```

正序排列也有关键字，为ASC，可被省略。

### 对多个数据表进行操作
需要指定一个关联的字段  
例，在两个表中查询所有的字段的值：
```
SELECT * FROM 表1, 表2 WHERE 表1.classId = 表2.classId
```
或者，在两个表中查询受关注的某几个字段
```
SELECT 表1.id, 表1.name, 表2.class_name FROM 表1, 表2 WHERE 表1.classId = 表2.classId
```
