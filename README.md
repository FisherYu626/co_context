# 用Boost库的asio包建立一个简单的echo server

## 已安装boost库
``` shell
/usr/local/include
``` 
### cmake configuration
``` cmake
FIND_PACKAGE(Boost)
```
### 启动echo server于指定端口
``` shell
./co_context 1234
```
### 用netcat启动一个tcp连接的客户端
``` shell
nc 127.0.0.1 1234
```