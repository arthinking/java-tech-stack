# 并发编程

## 在线资源

### 线程
- 关键词：`synchronized` `临界区` `自旋锁` `CAS` `TSL` `信号量` `互斥量` `ReentrantLock`
- 相关文章：
  - [一文带你彻底理解同步和锁的本质(干货)](https://www.itzhai.com/cpj/process-synchronization-and-lock.html)
  - [Chapter 15 Process & Thread & Synchronization](https://www.zybuluo.com/gone/note/35572)
  - [如何优雅的中断线程](https://www.itzhai.com/cpj/how-to-interrupt-threads-gracefully.html)
  - [如何优雅的挂起线程](https://www.itzhai.com/cpj/how-to-suspend-threads-gracefully.html)
- 相关问题：
  - 进程和线程通信的本质是什么？知道其原理吗？
  - synchronized锁是如何实现的？锁升级是个什么流程？锁优化又是什么流程？
  - 市面上各种锁都是什么意思？
  - stop方法为何被废弃了
  - 如何使用interrupt对线程进程中断
  - suspend和resume方法为何被废弃了？
  - 如何优雅的挂起线程

### 线程池

- 关键词：`线程池`
- 相关文章：
  - [一台java服务器可以跑多少个线程？](https://www.jianshu.com/p/f1930596947d)
- 相关问题：
  - 如何设置线程池数量？

### Java内存模型

- 关键词：`Java内存模型` `JMM` `volatile` `synchronized`
- 相关文章：
  - [如果有人给你撕逼Java内存模型，就把这些问题甩给他](https://www.itzhai.com/cpj/how-the-java-memory-model-works.html)
  - [小姐姐都能看懂的Happens-before规则，你还愣住了？](https://mp.weixin.qq.com/s/b-kZfWY0-VO95wts0sAo0w)
- 相关问题：
  - 什么是内存模型？为什么要有内存模型？
  - Java内存模型是怎样的？
  - Java内存模式如何实现多线程同步
  - volatile有什么用？什么时候需要用volatile？
  - 什么是指令重排？有什么用
  - final为何可以实现可见性？
  - synchronized是如何实现可见性的？
  - 如何保证原子性？什么是DCL并发问题？如何解决
  - Java内存模型中有哪些先行发生原则？

### 并发容器

- 关键词：`ConcurrentHashMap` `ConcurrentLinkedQueue`
- 相关文章：
  - [HashMap? ConcurrentHashMap? 相信看完这篇没人能难住你！](https://crossoverjie.top/2018/07/23/java-senior/ConcurrentHashMap/)
- 相关问题：
  - 请说说JDK1.7和JDK1.8中HashMap底层的数据结构？
  - 请说说JDK1.7和JDK1.8的ConcurrentHashMap分别是如何实现的？


### JUC
- 关键词：`ReentrantLock` `AQS` `JUC` `CountDownLatch` `CyclicBarrier` `Semaphore` `BlockingQueue` `ArrayBlockingQueue` `LinkedBlockingQueue` `LinkedBlockingDeque` `PriorityBlockingQueue` `SynchronousQueue` `DelayQueue`
- [AQS与并发包中锁的通用实现](https://www.itzhai.com/cpj/aqs-and-lock-implementation-in-concurrent-packages.html)
- [图解几个好玩的并发辅助工具类](https://www.itzhai.com/cpj/graphical-several-fun-concurrent-helper-classes.html)
- [图解BlockingQueue阻塞队列](https://www.itzhai.com/cpj/graphical-blocking-queue.html)
- [线程池ForkJoinPool简介](http://javakk.com/215.html)
  - 抽象同步器AQS的实现原理
  - ReentrantLock实现原理
  - 非公平锁和公平锁实现的区别
  - 可中断锁的实现原理
  - AQS的核心是state字段以及双端等待队列
  - CountDownLatch的工作原理和使用场景；
  - CyclicBarrier的工作原理和使用场景；
  - Semaphore的工作原理和使用场景。
  - 各种阻塞队列底层是如何实现的，他们之间有什么优缺点，在什么场景使用；

## 书籍

* :book: 《Java并发编程实战》
* :book: 《Java并发编程之美》
