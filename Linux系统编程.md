# Linux系统编程入门 [:fa-youtube-play:](https://www.nowcoder.com/study/live/504) 
***
***

### 1.GCC
- GCC的基础概念，gcc和g++的区别
- GCC的工作流程：预处理-编译-汇编-链接
- GCC常用参数

### 2.库
- 库的基本概念，静态库和动态库的区别
- 静态库：命名规则、制作
- 动态库：命名规则、制作
- 静态库和动态库的对比

### 3.Makefile
- Makefile基本概念、文件命名和规则
- Makefile工作原理
- Makefile变量：自定义变量、预定义变量、获取变量的值
- 模式匹配
- 函数

### 4、GDB调试
- GDB调试工具基本概念、功能、准备工作
- GDB命令： **启动、退出、查看代码、断点操作**  :fa-star-o: 
- GDB命令-调试命令： **运行GDB程序（start、run）、继续运行，到下一个断点停（c/continue）、向下执行一行代码（n/next）、变量操作（p/print 变量名、ptype 变量名）、向下单步调试（s/step、finish）、自动变量操作（display num、i/info display、undisplay 编号）、其他操作（set var 变量名=变量值、until）**  :fa-star: 

### 5.Linux文件IO
- 了解 **标准C库IO函数** 
- 了解 **标准C库IO和Linux系统IO的关系** 
- 了解 **虚拟地址空间** 
- 了解 **文件描述符** 的概念
- 了解Linux系统IO函数：open函数、close函数、read函数、write函数、lseek函数、stat函数、lstat函数、


***
***
# Linux多进程开发
***
***

### 1.进程
- 了解 **程序** 和 **进程** 的概念；了解时间片的概念；了解并行和并发的概念；了解 **进程控制块（PCB）** 的概念
- 了解 **进程的状态切换** ；了解 **进程相关命令** ；了解 **进程号和相关函数** 
- 熟悉进程创建：fork
- 




***
***
# Linux多线程开发
***
***
-  [:fa-file-o: CSDN](https://blog.csdn.net/qq_41511474/article/details/130215159?csdn_share_tail=%7B%22type%22%3A%22blog%22%2C%22rType%22%3A%22article%22%2C%22rId%22%3A%22130215159%22%2C%22source%22%3A%22qq_41511474%22%7D&fromshare=blogdetail)

***
***
# Linux网络编程
***
***

暂无




***
***
# 项目实战——Web服务器
***
***




### 1.阻塞/非阻塞、同步/异步(网络IO) [ :fa-file-text-o: ](https://blog.csdn.net/hguisu/article/details/7453390?ops_request_misc=&request_id=&biz_id=102&utm_term=%E9%98%BB%E5%A1%9E/%E9%9D%9E%E9%98%BB%E5%A1%9E&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-4-7453390.142^v86^insert_down38v5,239^v2^insert_chatgpt&spm=1018.2226.3001.4187)

> 典型的一次IO的两个阶段是什么？ **数据就绪** 和 **数据读写** 

- 数据就绪：根据系统IO操作的就绪状态
    - 阻塞
    - 非阻塞
- 数据读写：根据应用程序和内核的交互方式
    - 同步
    - 异步

> 一个典型的网络IO接口调用，分为两个阶段，分别是“数据就绪” 和 “数据读写”，数据就绪阶段分为阻塞和非阻塞，表现得结果就是，阻塞当前线程或是直接返回。

> 同步表示A向B请求调用一个网络IO接口时（或者调用某个业务逻辑API接口时），数据的读写都是由请求方A自己来完成的（不管是阻塞还是非阻塞）；异步表示A向B请求调用一个网络IO接口时（或者调用某个业务逻辑API接口时），向B传入请求的事件以及事件发生时通知的方式，A就可以处理其它逻辑了，当B监听到事件处理完成后，会用事先约定好的通知方式，通知A处理结果。

> 陈硕：在处理 IO 的时候，阻塞和非阻塞都是同步 IO，只有使用了特殊的 API 才是异步 IO。

### 2.Unix/Linux上的五种IO模型 [ :fa-file-text-o: ](https://blog.csdn.net/lpf463061655/article/details/103403466?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522168311456716800180630150%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=168311456716800180630150&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-1-103403466-null-null.142^v86^insert_down38v5,239^v2^insert_chatgpt&utm_term=linux%20io%E6%A8%A1%E5%9E%8B&spm=1018.2226.3001.4187)
- 熟悉IO模型： **阻塞 blocking、非阻塞 non-blocking（NIO）、IO复用（IO multiplexing）、信号驱动（signal-driven）、异步（asynchronous）** 





### 3.Web服务器简介

- 熟悉Web服务器的概念 [ :fa-file-text-o: ](https://blog.csdn.net/HelloZEX/article/details/122810557?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522168311565316782425181872%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=168311565316782425181872&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-1-122810557-null-null.142^v86^insert_down38v5,239^v2^insert_chatgpt&utm_term=Web%E6%9C%8D%E5%8A%A1%E5%99%A8%E7%9A%84%E6%A6%82%E5%BF%B5&spm=1018.2226.3001.4187)
![输入图片说明](pics/Screenshot%202023-05-02%20220648.png)

- 熟悉HTTP协议 [ :fa-file-text-o: ](https://blog.csdn.net/qq_36894974/article/details/103930478?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522168311478816800226552390%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=168311478816800226552390&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_positive~default-1-103930478-null-null.142^v86^insert_down38v5,239^v2^insert_chatgpt&utm_term=HTTP%E5%8D%8F%E8%AE%AE&spm=1018.2226.3001.4187)

### 4.服务器编程基本框架和两种高效的事件处理模式 [ :fa-file-text-o: ](https://blog.csdn.net/weixin_47468969/article/details/124536503?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522168311572116800226518629%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=168311572116800226518629&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-1-124536503-null-null.142^v86^insert_down38v5,239^v2^insert_chatgpt&utm_term=%E6%9C%8D%E5%8A%A1%E5%99%A8%E7%BC%96%E7%A8%8B%E5%9F%BA%E6%9C%AC%E6%A1%86%E6%9E%B6&spm=1018.2226.3001.4187)

- 熟悉服务器基本框架
![输入图片说明](pics/Screenshot%202023-05-02%20222208.png)
![输入图片说明](pics/Screenshot%202023-05-02%20222102.png)

- 熟悉两种高效的事件处理模式： **Reactor模式、Proactor模式** 

### 5.线程池
- 熟悉线程池的概念 [ :fa-file-text-o: ](https://blog.csdn.net/qq_43061290/article/details/106911277?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522168311631416800222892090%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=168311631416800222892090&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_positive~default-2-106911277-null-null.142^v86^insert_down38v5,239^v2^insert_chatgpt&utm_term=%E7%BA%BF%E7%A8%8B%E6%B1%A0&spm=1018.2226.3001.4187)























