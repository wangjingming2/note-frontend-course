npm是node内置的包管理器  
可以使用npm下载并安装别人写的命令行工具来使用  
npm官网：www.npmjs.com  
国内的npm镜像网站：npm.taobao.org

简单的服务器  
```
var http = require('http');
http.createServer(function(req, res){
    res.writeHead(200, {'Content-Type':'text/plan'});
    res.end('Hello world!\n');
}).listen(8000);

console.log('server is running...');
```