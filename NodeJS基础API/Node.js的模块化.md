一个文件就是一个模块  
这个文件可能是JavaScript代码、JSON或者编译过的c/c++扩展  
[nodejs的模块加载流程](./img/nodejs的模块加载流程.png)

### require方法加载模块的方式
require方法接受以下几种参数的传递：
1. http, fs, path等，原生模块
2. ./mod或../mod，相对路径的文件模块
3. /pathtomodule/mod，绝对路径的文件模块
4. 非原生模块的文件模块

例：
```
// 引入自己写的模块
require('./name');

```