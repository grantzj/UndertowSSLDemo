#项目简介
- 1.这是一个简单的Spring-Boot项目，使用了Undertow作为容器。
- 2.配置了用JDK的keytool.exe本地生成的SSL证书。
- 3.为Undertow配置了多端口监听，分别监听8080(http)、9090(https)，并将http请求后台重定向到https接口。
- 4.同时开通了Undertow的http2.0功能。
- 5.项目提供了一个get类型的对外接口，启动后可以用于http和https类型的请求测试：
> https://127.0.0.1:9090/undertowSslDemo/user/getUser?id=99
> http://127.0.0.1:8080/undertowSslDemo/user/getUser?id=99
#目的
- 住要学习Spring-Boot之web项目对的https支持。
