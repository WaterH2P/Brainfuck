## 包划分

客户端：BF/src

​	/rmi		RMI工具类

​	/runner         启动类

​	/service         服务器提供的接口

​	/ui                  GUI

 

服务器：BFServer/src

​	/rmi                        RMI工具类

​	/runner               启动类

​	/service                  服务器提供的接口

​	/serviceImpl          服务的具体实现

 

## 注意

1. 先启动服务器，再启动客户端
2. 如果要使用RMI进行网络通信，客户端和服务器对应的接口需要一致，即两个项目下的/service下的接口需要一致
3. BFServer/src/serviceImpl/ExecuteServiceImpl.java文件的文件名，以及excute方法的声明不要修改，最终我们会通过这个方法测试解释器实现的正确性