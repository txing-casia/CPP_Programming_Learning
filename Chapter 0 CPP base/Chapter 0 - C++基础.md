##Chapter 0 C++基础

工具：

- /usr/bin/time sleep 1: 系统停止1毫秒，/usr/bin/time是监控程序运行时间的命令行
- valgrind: 内存泄露检测；

一些网站：

- cppreference.com：较权威的C++百科全书，命令查询；

- compiler explorer：汇编代码生成并运行，自由选择编译器，不同版本编译器对比；

- Cppinsights：生成等价代码解释；

- youtube CppCon：C++相关技术的会议；

C++编译：

- 分块编译机制，减少资源消耗
- 便于修改
- 头文件/源文件
- 翻译单元：源文件+相关头文件-应忽略的预处理语句
- 编译文件为可执行文件：g++ ./main.cpp -o ./main
- 防止头文件循环展开：
  - #ifndef方案，如果没有编译该头文件，则编译该头文件；
  - #pragma once方案，（比较好的方案）只编译一次该头文件；
- Debug编译引入优化较少
- Release编译引入优化较多
- 增量编译 & 全部编译
- 连接（Linkage）种类：内部连接、外部连接、无连接
- C++程序预处理、编译、链接都可能出错



