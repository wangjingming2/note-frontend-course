1. PHP只能够继承一个父类，能够实现多个接口
2. 在子类中使用parent来访问被重写的父类方法
3. PHP不支持重载

实例：
```
class Person
{
    function __construct(p1, p2){}
}

class Yellow exctends Person
{
    function __construct(p1, p2)
    {
        parent::__construct(p1, p2)
    }
}
```