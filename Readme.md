# Java核心基础
## Java基础
*    [谈谈你对Java平台的理解](doc/java_core_tech/1.谈谈你对Java平台的理解.md)
*    Exception和Error有什么区别
*    谈谈final、finally、finalize有什么不同
*    强引用、软引用、弱引用、幻象引用有什么区别
*    String、StringBuffer、StringBuilder有什么区别
*    动态代理是基于什么原理
*    int和Integer有什么区别
*    对比Vector、ArrayList、LinkedList有何区别
*    对比Hashtable、HashMap、TreeMap有什么不同
*    如何保证集合是线程安全的（ConcurrentHashMap如何实现高效地线程安全）
*    Java提供了哪些IO方式（NIO如何实现多路复用）
*    Java有几种文件拷贝方式（哪一种最高效）
*    谈谈接口和抽象类有什么区别
*    谈谈你知道的设计模式

## Java进阶
*    synchronized和ReentrantLock有什么区别呢
*    synchronized底层如何实现（什么是锁的升级、降级）
*    一个线程两次调用start()方法会出现什么情况
*    什么情况下Java程序会产生死锁（如何定位、修复）
*    Java并发包提供了哪些并发工具类
*    并发包中的ConcurrentLinkedQueue和LinkedBlockingQueue有什么区别
*    Java并发类库提供的线程池有哪几种（分别有什么特点）
*    AtomicInteger底层实现原理是什么？如何在自己的产品代码中应用CAS操作
*    请介绍类加载过程，什么是双亲委派模型
*    有哪些方法可以在运行时动态生成一个Java类
*    谈谈JVM内存区域的划分（哪些区域可能发生OutOfMemoryError）
*    如何监控和诊断JVM堆内和堆外内存使用
*    Java常见的垃圾收集器有哪些
*    谈谈你的GC调优思路
*    Java内存模型中的happen-before是什么
*    Java程序运行在Docker等容器环境有哪些新问题

## Java安全基础
*    你了解Java应用开发中的注入攻击吗
*    如何写出安全的Java代码

## Java性能基础
*    后台服务出现明显“变慢”，谈谈你的诊断思路
*    有人说“Lambda能让Java程序慢30倍”，你怎么看

## Java应用开发扩展
*    JVM优化Java代码时都做了什么
*    谈谈MySQL支持的事务隔离级别，以及悲观锁和乐观锁的原理和应用场景

---
# 深入理解Java虚拟机
## 基本原理
*   Java代码是怎么运行的  
    Java虚拟机的意义、Java字节码、Java虚拟机的运行效率
*   Java基本类型  
    Java虚拟机的boolean类型、Java的基本类型、Java基本类型的大小
*   JVM是如何加载Java类的  
    加载、链接、初始化
*   JVM是如何执行方法调用的（一）  
    重写与重载、静态绑定与动态绑定、调用指令的符号引用
*   JVM是如何执行方法调用的（二）  
    虚方法调用、方法表、内联缓存方法表、内敛缓存
*   JVM是如何实现反射的  
    反射API简介、反射调用的实现、反射调用的性能开销
*   Java8的Lambda表达式是怎么运行的  
    动态语言与Lambda、invokedynamic指令和method handle、invokedynamic指令的运行效率
*   JVM构造对象的步骤有哪些  
    构造对象的步骤、new指令的实现、JVM堆的区域划分
*   什么是垃圾收集  
    自动管理内存的意义、垃圾收集算法、如何选择垃圾收集算法
*   JVM是如何实现同步的  
    synchronized关键字的实现、JVM的锁算法、cocurrent核心库
*   Java内存模型是什么  
    多处理器架构下的内存读写、happens-before原则、volatile关键字、对象的安全发布
*   JVM的安全点是什么  
    安全点的概念、安全点的位置、JVM何时使用安全点


## 高效实现
*   javac是如何编译Java源代码的  
    自动装箱与自动拆箱、变长参数、foreach循环、范型与类型擦出、桥接方法
*   如何使用注解解释器  
    注解与元数据、Java核心类库中的标准注解、自定义注解
*   解释器如何触发即时编译  
    即时编译简介、触发即时编译的时机、生成代码的性能
*   即时编译器与常规的静态编译器有哪些不同  
    profiling、基于程序profile的优化方式、去优化
*   即时编译器有哪些优化  
    强度削弱
*   在什么情况下重复读写操作会被优化  
    读写删除优化
*   在什么情况下循环代码会被优化  
    循环展开、其他循环优化、OSR编译
*   什么情况下对象分配会被优化  
    逃逸分析、栈分配、标量替换
*   在什么情况下方法调用会被内联  
    方法内联的概念、完全去虚化、条件去虚化
*   什么是intrinsics，为什么它们非常高效  
    JVM中intrinsics的概念、intrinsics的性能
*   如何写出适用向量化计算的代码  
    SIMD指令集、JVM的自动向量化优化、如何写出适用向量化的代码


## 代码优化
*   如何理解JVM内置的编译或GC日志  
    编译日志、GC日志、去优化日志
*   如何利用JFR和JMC监控Java程序  
    Java Flight Recorder简介、Java Mission Control简介
*   如何利用MAT分析Java程序的堆使用情况  
    内存泄漏、Eclipse MAT内存分析工具
*   如何利用JMH评估代码性能  
    JMH的意义、JMH的应用
*   如何在Java代码中与C++代码交互  
    Java Native Interface简介、Native方法与链接、在C++代码中调用Java方法、Java Native Access简介
*   如何利用JVMTI监听JVM事件  
    JVM Tool Interface简介、监听JVM事件
*   如何利用字节码注入为已有代码加料  
    字节码注入工具、Java agent与C agent、面向方面的编程方式
*   如何利用Unsafe API绕开JVM的控制  
    Unsafe API简介、Unsafe的风险


## 虚拟机黑科技
*   Graal：用Java编译Java  
    Graal和JVM的交互、Graal和C2的区别、Graal的实现
*   Truffle：用Java编译其他语言  
    Partical Evaluator、抽象语法书及其解释器、同时使用多种语言的Polyglot
*   SubstrateVM：用Java编译虚拟机  
    AOT编译、SubstrateVM的实现与局限、SubstrateVM的应用场景
*   Metropolis：Java-on-Java的展望  