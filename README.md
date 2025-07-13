Welcome to nanomsg
==================

[![Release](https://img.shields.io/github/release/nanomsg/nanomsg.svg)](https://github.com/nanomsg/nanomsg/releases/latest)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/nanomsg/nanomsg/blob/master/COPYING)

nanomsg库是几个组件的简单高性能实现“可扩展性协议”。这些可扩展性协议是轻量级的消息传递可用于解决许多非常常见的消息传递的协议模式，如请求/回复、发布/订阅、调查员/受访者，等等。这些协议可以在各种传输上运行，例如TCP、UNIX套接字，甚至WebSocket。

构建
------------------------

cmake常规构建步骤即可
```
mkdir build
cd build
cmake ..
make 
make install
```

集成至tinyPiXOS
------------------------

- 生成文件在install/目录
- 拷贝/install/include/nanomsg/* -> tinyPiXCore/src/include_p/Utils/nanomsg
- 拷贝/install/lib/libnanomsg.a -> tinyPiXCore/src/depend_lib/static/x86_x64(根据平台拷贝至x86或arm目录)
