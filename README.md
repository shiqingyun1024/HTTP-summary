# HTTP-summary
HTTP网络协议相关的总结
## HTTP请求头中包含的内容
```
Host: www.study.com                // 请求的地址域名和端口，不包括协议

Connection: keep-alive　　　   // 连接类型，持续连接

Upgrade-Insecure-Requests：1  // http 自动升级到https，防止跨域问题但是域名端口都不同的不会提升

User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.96 Safari/537.36  //浏览器的用户代理信息

Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,`*/*`;q=0.8     //浏览器支持的请求类型

Accept-Encoding: gzip, deflate, sdch   //浏览器能处理的压缩代码

Accept-Language: zh-CN,zh;q=0.8,en;q=0.6  //浏览器当前设置语言

Content-Length: 29                  //请求参数长度
Cache-Control: max-age=0      //强制要求服务器返回最新的文件内容,也就是不走缓存，返回的200
Origin: http://www.study.com    //请求来源地址，包括协议

Referer: http://www.study.com/day02/01-login.html     //原始的url,不带锚点，比方说在谷歌打开百度，feferer显示的是谷歌的url
```