# AIDL

### AIDL的全称是什么?

Android Interface Define Language

**主要用来处理进程间通信 (IPC), 也就是两个安卓应用程序之间的通信.**

### 如何工作?

核心是代理类和绑定服务. 

* 在服务端编写的AIDL文件, 编译时会自动生成一个 java 文件, 该文件里有一个代理类, 实质是通过这个代理类和客户端进行通信.
* 然后咋服务端创建一个服务, 监听请求, 其实也就是让客户端绑定这个服务, 从而能交互.
* 客户端要创建一个相同的AIDL文件.
* 在程序里绑定服务, 通过服务返回的 binder 与远程服务进行交互.





