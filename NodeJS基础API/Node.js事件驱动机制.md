node使用的是[事件驱动模型](./img/事件驱动模型.png)

### 事件处理代码流程
1. 引入events对象，创建eventEmitter对象
2. 绑定事件处理程序
3. 触发事件

例：
```
// 引入Event模块并创建evnetEmitter对象
var events = require('event');
var eventEmitter = new events.EventEmitter();

// 绑定事件处理函数
var connectHandler = function connected(){
    console.log('connected 被调用！');
};

eventEmitter.on('connection', connectHandler;

// 触发事件
eventEmitter.emit('connection');

console.log('程序执行完毕');

```