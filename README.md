# hello-world
2. PrixyHander处理器（代理）：

   1. 代理的原理， 先请求代理服务器， 然后让代理服务器去请求目的网站， 代理服务器拿到目的网站数据后， 再转发到我们的代码

   2. http:/httpbin.org可以方便查看http请求的一些参数

   3. 代码中使用代理

      - 使用："urllib.request.proxyHandler",传入一个代理， 代理是一个子弹， 字典key依赖于代理服务器能够接受的类型， 一般式“http”， “https”值是“ip:port”

      - 使用上一步的：“Handler", 以及”request.build_opener“创建一个”opener“对象

      - 使用上一部的：opener， 调用open函数
