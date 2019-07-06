可以通过扩展Exception异常类来定义自己的异常类。使用自定义的异常类的时候可以像如下这样
```
class myException extends Exception
{
    public function getAllInfo() {
        return "xxxxx";
    }
}

try{
    throw new myException();
} catch(myException $e) {
    echo $e->getAllInfo();
}
```
一个try语句可以后接多个catch语句来捕捉多种不同的异常