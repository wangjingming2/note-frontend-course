1. 引入外部文件：require_once('a.php');
2. 引入外部文件：include_once('a.php);
3. require_once和include_once的区别就是：使用require_once引入的文件必须的，如果不能正常引入这个文件那么当前文件内的程序就会报错；使用include_once引入的文件不是必须的，当没有正常引入外部文件时，只有在使用了这个外部文件内的变量等的时候才会报错
4. $GLOBALS用于在全局声明声明一个变量：$GLOBALS['a']声明了一个全局的a变量
5. 声明数组：$arrayTest = array('0'=>"苹果", 1=>"测试");
6. json_encode($arrayTest)使用json格式输出字符串
7. 操作session。在使用session的时候一定要调用session_start()才能开始使用session，除非在服务器上配置。
8. 设置session:  
   session_start();  
   $_SESSION['xxx'] = 1;
9. 读取session：session_start();  
   $SESSION['XXX']
10. 处理表单：  
    $_GET['XXX'];得到使用get方法提交的参数  
    $_POST['XXX'];得到使用post方法提交的数据:  
    $_REQUEST['XXX'];得到get或者post方法提交的数据
11. 在PHP页面中使用header();设置字符编码  
    header('Content-type:text/html;charset=utf-8');
12. $.ajax中的error处理的是连接错误，而不是服务器处理的错误
13. 在$.ajax中的data中如果有个字段是undefined，那么就不会提交这个字段，或者说是忽略这个字段
14. PHP响应json数据请求也是通过echo关键字