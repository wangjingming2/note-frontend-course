interface 接口名称 {
	常量成员
	抽象方法
}

例：
```
interface Person{
    const NAME = "xiaowang";
    public function run();
}
```
运算符用于访问类的静态成员和类常量，也可以用来引用父类被覆盖的方法
在类外使用：
```
$aaa::b
```
在类内使用：
```
parent::aa
self::aa
```