1. PHP与MySQL连接：mysql_connect(servername, username, password);返回一个连接
2. 关闭连接：mysql_close(connect);
3. 连接数据库的时候一定要做错误判断
```
    $con = mysql_connect("localhost", "root", "123");
    if (!$con) {
        die("Could not connect: ", mysql_error());
    }else {
        echo "mysql connect ok";
        // 选择要操作的数据库
        mysql_select_db("数据库名字", connect);
        mysql_query("select * from news", $con);
        // 操作数据库的数据
        mysql_query("数据库操作命令");
        mysql_close(connect);
    }
```
4. 数据库操作的时候也需要做容错处理  
   $query = mysql_query("数据库操作命令");  
   if(!query){echo mysql_error();}else{}
5. 在与数据库交互的时候注意设置字符编码的格式  
   mysql_query("set names 'utf-8'");
6. 数据库操作命令 
``` 
   // 插入数据  
   INSERT INTO '表的名字' ('字段1', '字段2', '字段3') VALUES ('字段1的值', '字段2的值', '字段3的值');  
   //删除数据  
   DELETE FROM 表的名字 WHERE 字段名=值  
   // 更新数据  
   UPDATE 表的名字 SET  '字段名=值', '字段名=值' WHERE 条件表达式
```