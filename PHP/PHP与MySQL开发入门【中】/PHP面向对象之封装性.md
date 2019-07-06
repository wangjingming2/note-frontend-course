PHP5支持关键字：
public
private
protected

魔术方法  
`__set($key, value)`：设置某个属性的时候会执行  
`__get($key)`：得到某个属性的时候会执行  
`__isset($key)`：判断是否能够访问某个属性  
`__unset($key)`：删除某个属性的时候会执行  
是对private和protected的成员进行操作的