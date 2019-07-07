### 什么是回调
函数调用方式分为三类：同步调用、回调和异步调用。
回调是一种双向调用模式
可以通过回调函数来实现回调

阻塞方法
```
var fs = require('fs');
var data = fs.readFileSync('data.txt');
// 读取过来的数据是二进制形式的需要处理一下变成字符串
console.log(data.toString());
```

非阻塞方法
```
var fs = require('fs');
var data = fs.readFile('data.txt', function(error, data){
    if (error) {
        // 进行容错处理
    } else {
        // some code...
    }
});
```