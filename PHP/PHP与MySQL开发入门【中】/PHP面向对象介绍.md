用于引用$aaa对象中的bbb成员变量
```
$aaa -> bbb;
```
用于对$aaa对象中的bbb成员变量赋值
```
$aaa -> bbb = ccc
```
调用$aaa对象中的bbb方法
```
$aaa->bbb()
```

this的使用
```
$this
```

类的声明
\[修饰符\] class 类名\[extends 父类\]\[implements 接口1\[, 接口2…\]\]  
\{  
    \[成员属性\]  
    \[成员方法\]  
\}  
例：
```
public class A extends B implements C {
    public $d;
    public $e = 'aaa';
    public $f = self::bbb  // 静态属性
    public function ggg ($p) {}
}
```