## HTTP 的方法有哪些？

+ GET：    一般用于获取数据；
+ HEAD：   类似于GET请求，只不过返回的响应中没有具体的内容，用户获取报文头；  
+ POST：   一般用于创建资源或修改资源；
+ PUT：    替换指定的资源，如果没有就新增；
+ DELET：  请求服务器删除URL标识的资源数据；
+ CONNECT：将服务器作为代理，让服务器代替用户访问；
+ OPTION： 想服务器发送该方法，会返回对指定资源所支持的HTTP请求方法；
+ TRACE：  回显服务器收到的请求数据，即服务器返回自己收到的数据，主要用于测试和诊断；
+ PATCH：  是PUT方法的补充，用来对已知资源进行局部更新；