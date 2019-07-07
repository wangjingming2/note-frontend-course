[路由的方法对应的返回值](./img/nodejs路由的一些方法的作用.png)

```
var http = require("http");
var url = require("url");
http.createServer(function(req, res){
    url.parse(req.url).pathname;
    //...
}).listen(8888);

```