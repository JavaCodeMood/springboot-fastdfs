FastDFS      
-
源码： GItHub地址：https://github.com/happyfish100    

搭建FastDFS: https://blog.csdn.net/wlwlwlwl015/article/details/52619851


FastDFS是一个开源的轻量级分布式文件系统，它对文件进行管理，功能包括：文件存储、文件同步、文件访问（文件上传、文件下载）等，解决了大容量存储和负载均衡的问题。特别适合以文件为载体的在线服务，如相册网站、视频网站等等。

FastDFS的两个核心概念分别是：Tracker（跟踪器）、Storage（存储节点）

适用场合
-
特别适合以文件为载体的在线服务，如相册网站、视频网站等等。

组成部分及其作用
-
FastDFS客户端，其作用是完成客户与服务端之间的交互。

FastDFS服务端，有两个角色：

a.跟踪器（tracker），其作用是完成调度工作，在访问上起负载均衡的作用。

b.存储节点（storage），其作用是完成文件的存储，完成文件管理的所有功能：存储、同步和提供存取接口，FastDFS同时对文件的meta data进行管理。所谓文件的meta data就是文件的相关属性，以键值对（key value pair）方式表示，如：width=1024，其中的key为width，value为1024。文件metadata是文件属性列表，可以包含多个键值对。


