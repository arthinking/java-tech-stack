# Java并发编程系列文章

### Java内存模型
- 相关文章：
  - [如果有人给你撕逼Java内存模型，就把这些问题甩给他](https://www.itzhai.com/cpj/how-the-java-memory-model-works.html)
- 关键词：`Java内存模型` `JMM` `volatile` `synchronized`
- 相关问题：
  1. 什么是内存模型？为什么要有内存模型？
  2. Java内存模型是怎样的？
  3. Java内存模式如何实现多线程同步
  4. volatile有什么用？什么时候需要用volatile？
  5. 什么是指令重排？有什么用
  6. final为何可以实现可见性？
  7. synchronized是如何实现可见性的？
  8. 如何保证原子性？什么是DCL并发问题？如何解决
  9. Java内存模型中有哪些先行发生原则？

### 同步和锁的本质
- 相关文章：
  - [一文带你彻底理解同步和锁的本质(干货)](https://www.itzhai.com/cpj/process-synchronization-and-lock.html)
- 关键词：`synchronized` `临界区` `自旋锁` `CAS` `TSL` `信号量` `互斥量` `ReentrantLock`
- 相关问题：
  1. 进程和线程通信的本质是什么？知道其原理吗？
  2. synchronized锁是如何实现的？锁升级是个什么流程？锁优化又是什么流程？
  3. 市面上各种锁都是什么意思？意思？

### 线程中断
- 相关文章：
  - [如何优雅的中断线程](https://www.itzhai.com/cpj/how-to-interrupt-threads-gracefully.html)
- 关键词：`interrupt` `stop`
- 相关问题：
  1. stop方法为何被废弃了
  2. 如何使用interrupt对线程进程中断

### 线程挂起
- 相关文章：
  - [如何优雅的挂起线程](https://www.itzhai.com/cpj/how-to-suspend-threads-gracefully.html)
- 关键词：`suspend`
- 相关问题：
  1. suspend和resume方法为何被废弃了？
  2. 如何优雅的挂起线程

### AQS并发包中的锁
- 相关文章：
  - [AQS与并发包中锁的通用实现](https://www.itzhai.com/cpj/aqs-and-lock-implementation-in-concurrent-packages.html)
- 关键词：`ReentrantLock` `AQS` `JUC`
- 相关问题：
  1. 抽象同步器AQS的实现原理
  2. ReentrantLock实现原理
  3. 非公平锁和公平锁实现的区别
  4. 可中断锁的实现原理
  5. AQS的核心是state字段以及双端等待队列

### 并发辅助工具类
- 相关文章：
  - [图解几个好玩的并发辅助工具类](https://www.itzhai.com/cpj/graphical-several-fun-concurrent-helper-classes.html)
- 关键词：`CountDownLatch` `CyclicBarrier` `Semaphore`
- 相关问题：
  1. CountDownLatch的工作原理和使用场景；
  2. CyclicBarrier的工作原理和使用场景；
  3. Semaphore的工作原理和使用场景。


### 阻塞队列
- 相关文章：
  - [图解BlockingQueue阻塞队列](https://www.itzhai.com/cpj/graphical-blocking-queue.html)
- 关键词：`BlockingQueue` `ArrayBlockingQueue` `LinkedBlockingQueue` `LinkedBlockingDeque` `PriorityBlockingQueue` `SynchronousQueue` `DelayQueue`
- 相关问题：
  1. 各种阻塞队列底层是如何实现的，他们之间有什么优缺点，在什么场景使用；

### 并发容器


### 线程池
