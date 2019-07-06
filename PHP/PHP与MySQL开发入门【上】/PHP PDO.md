PDO是PHP与数据库进行连接的技术
```
<?php
    header("Content-Type: text/html;charset=utf-8);
    $dbms = "mysql";
    $host = "localhost";
    $dbname = "yideng";
    $user = "root";
    $pass = "";
    $dsn = "$dbms:host=$host;dbname=$dbName";

    try{
        $dbh = new PDO($dsn,$user,$pass);
        echo "连接成功<br/>";

        foreach($dbh->query("SELECT * FROM `news` WHERE 1") as $row){
            print_r($row);
        }
        
    }catch(PDOException $e){
        die("Error:".$e.getMessage()."</br/>");
    }
?>
```