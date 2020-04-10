# Java并发编程系列文章

### 并发知识体系



### Java内存模型

- 关键词：`Java内存模型` `JMM` `volatile` `synchronized`
- [如果有人给你撕逼Java内存模型，就把这些问题甩给他](https://www.itzhai.com/cpj/how-the-java-memory-model-works.html)
  - 什么是内存模型？为什么要有内存模型？
  - Java内存模型是怎样的？
  - Java内存模式如何实现多线程同步
  - volatile有什么用？什么时候需要用volatile？
  - 什么是指令重排？有什么用
  - final为何可以实现可见性？
  - synchronized是如何实现可见性的？
  - 如何保证原子性？什么是DCL并发问题？如何解决
  - Java内存模型中有哪些先行发生原则？

### 进程/线程同步
- 关键词：`synchronized` `临界区` `自旋锁` `CAS` `TSL` `信号量` `互斥量` `ReentrantLock`
- [一文带你彻底理解同步和锁的本质(干货)](https://www.itzhai.com/cpj/process-synchronization-and-lock.html)
  - 进程和线程通信的本质是什么？知道其原理吗？
  - synchronized锁是如何实现的？锁升级是个什么流程？锁优化又是什么流程？
  - 市面上各种锁都是什么意思？意思？

### 线程-线程状态
- [Chapter 15 Process & Thread & Synchronization](https://www.zybuluo.com/gone/note/35572)

### 线程-线程中断
- 关键词：`interrupt` `stop`
- [如何优雅的中断线程](https://www.itzhai.com/cpj/how-to-interrupt-threads-gracefully.html)
  - stop方法为何被废弃了
  - 如何使用interrupt对线程进程中断

### 线程-线程挂起
- 关键词：`suspend`
- [如何优雅的挂起线程](https://www.itzhai.com/cpj/how-to-suspend-threads-gracefully.html)
  - suspend和resume方法为何被废弃了？
  - 如何优雅的挂起线程

### JUC中的同步机制-AQS并发包中的锁
- 关键词：`ReentrantLock` `AQS` `JUC`
- [AQS与并发包中锁的通用实现](https://www.itzhai.com/cpj/aqs-and-lock-implementation-in-concurrent-packages.html)
  - 抽象同步器AQS的实现原理
  - ReentrantLock实现原理
  - 非公平锁和公平锁实现的区别
  - 可中断锁的实现原理
  - AQS的核心是state字段以及双端等待队列

### JUC中的同步机制-并发辅助工具类
- 关键词：`CountDownLatch` `CyclicBarrier` `Semaphore`
- [图解几个好玩的并发辅助工具类](https://www.itzhai.com/cpj/graphical-several-fun-concurrent-helper-classes.html)
  - CountDownLatch的工作原理和使用场景；
  - CyclicBarrier的工作原理和使用场景；
  - Semaphore的工作原理和使用场景。

### JUC中的同步机制-阻塞队列
- 关键词：`BlockingQueue` `ArrayBlockingQueue` `LinkedBlockingQueue` `LinkedBlockingDeque` `PriorityBlockingQueue` `SynchronousQueue` `DelayQueue`
- [图解BlockingQueue阻塞队列](https://www.itzhai.com/cpj/graphical-blocking-queue.html)
  - 各种阻塞队列底层是如何实现的，他们之间有什么优缺点，在什么场景使用；

### 并发容器

* 关键词：`ConcurrentHashMap` `ConcurrentLinkedQueue`
* [HashMap? ConcurrentHashMap? 相信看完这篇没人能难住你！](https://crossoverjie.top/2018/07/23/java-senior/ConcurrentHashMap/)
  * 请说说JDK1.7和JDK1.8中HashMap底层的数据结构？
  * 请说说JDK1.7和JDK1.8的ConcurrentHashMap分别是如何实现的？


### 线程池

* 关键词：