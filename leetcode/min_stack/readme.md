- 数组的操作
    1. push pop 入栈出栈操作
    只在栈顶操作
    2. unshift shift 队列操作
    只在队头和队尾操作 FIFO
    CPU 的底层 
        写代码，放音乐，聊天 都是进程，分时分片 CPU 计算 分时 运行时钟

程序是怎么运行的？程序会崩溃
代码文本 文件系统fs
a.c 编译器 a.o 文件 可执行的程序文件 -> 内存 I/O CPU 分配空间 成为独立的进程
365？ 
 排队 空间不够
进程三个状态 
    执行 就绪 阻塞
顺序执行 代码是程序

程序崩溃？
CPU 分时分片 切换操作 Tomcat 独立的进程 进程切换很耗时
线程 可被独立运行的， 
web
 Tomcat 多线程
分布式

1. 冯诺依曼原理
    代码文件 -> compile -> 可执行文件 文件系统
2. CPU的分时分片计术
    执行可执行文件
    进程 由操作系统负责调度
    并行执行 多个进程在CPU切换
3. 进程切换消耗打，
    线程 
    *.java *.javac 启动多线程
4. Tomcat
    每个访问者new一个线程
    每个线程有独立的资源，内存，占据越来越多的内存空间，不释放，处于阻塞状态
    - 分配的线程数Tomcat的上线
    - 线程为了就绪，分配的内存达到服务器的物理上限时，也会死
5. 分布式的概念
    nginx 动态扩容 加服务器，负载均衡
