```
$sql = "selcet * from news";
mysql_query("set names 'utf-8'");
$result = mysql_query($sql, $con);
//创建一个数组
$arr = array();
while($row = mysql_fetch_array($result)) {
    //数组的push操作
    array_push($arr, array("newstitle"=>$row['newstitle'], "newsimg"=>$row['newsimg']));
}
echo json_encode($arr);
mysql_close($con);
```