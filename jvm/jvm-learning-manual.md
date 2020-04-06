# JVM系列文章

为了让JVM相关知识点能够形成一个**体系**，**arthinking**将编写整理一系列的专题，以尽量以图片的方式描述相关知识点，并且最终把所有相关知识点串成了一张图。

![image-20200214154250907](https://raw.githubusercontent.com/arthinking/java-tech-stack/master/jvm/assets/image-20200214154250907.png)

另外把文章列表和关键信息整理到下面了。

---

### Java运行时数据区域
- 相关文章：
  - [Java运行时数据区域是如何工作的](https://www.itzhai.com/jvm/how-java-runtime-data-area-works.html)
- 关键词：`JVM内存布局` `对象访问定位`
- 相关问题：
  - 1. JVM内存布局是怎么划分的？
  - 2. JVM里面各个区直接是怎么配合工作的？
  - 3. 对象在内存中是如何布局的？
  - 4. 什么是操作数栈和局部变量表？可否在class文件中展示下？
  - 5. 运行时常量和字符串常量有什么区别？
  - 6. 对象访问定位方式有哪些？各有什么优点

### Java垃圾回收机制
- 相关文章：
  - [Java垃圾回收机制](https://www.itzhai.com/jvm/java-garbage-collection-theory.html)
- 关键词：`可达性分析` `垃圾收集算法` `垃圾收集器`
- 相关问题：
  - 1. 一个对象的一生经历了什么？
  - 2. 如何判断对象是否可用？
  - 3. 引用计数法和可达性分析算法各有什么优缺点？
  - 4. 哪些对象可以作为GC ROOT？
  - 5. 垃圾回收的时候如何快速寻找到根节点？(安全点和OopMap)
  - 6. 垃圾回收算法有哪些？各有什么优缺点？
  - 7. 有哪些垃圾手气，各有什么优缺点，适用什么场景
  - 8. 何时触发MinorGC和MajorGC
  - 9. 什么是空间分配担保

### Java对象历险记
- 相关文章：
  - [Java对象历险记](https://www.itzhai.com/jvm/java-object-adventure.html)
- 关键词：`分配担保` `空间分配`
- 相关问题：
  - 1. Java对象进入堆之后，它的一生都经历了什么？

### Class文件
- 相关文章：[Class文件十六进制背后的秘密](https://www.itzhai.com/jvm/the-secret-of-hexadecimal-class-file.html)
- 关键词：`Class文件` `反汇编` `堆栈原理`
- 相关问题：
  - 1. 运行时常量池和静态常量池有什么区别？
  - 2. Class文件里面都有什么内容？
  - 3. Class文件反汇编之后的格式里面分别有什么，尝试解读里面方法中的汇编指令
  - 4. 本地变量表和操作数栈是如何工作的

### Class文件加载
- 相关文章：
  - [一篇图文彻底弄懂Class文件是如何被加载进JVM的](https://www.itzhai.com/jvm/how-class-file-load-into-jvm.html)
- 关键词：`类加载器` `加载` `连接` `初始化`
- 相关问题：
  - 1. Class.forName究竟是怎么获取Class对象的Class对象又是什么?
  - 2. Class文件是如何被加载到JVM里面的？
  - 3. 类变量是存在堆中还是存在方法区中?
  - 4. 类构造器`<clinit>`方法什么时候执行？

### 类加载器与双亲委派机制
- 相关文章：
  - [一篇图文彻底弄懂类加载器与双亲委派机制](https://www.itzhai.com/jvm/what-is-classloader-and-what-is-parents-delegation-model.html)
- 关键词：`类加载器` `双亲委派机制`
- 相关问题：
  - 1. 类加载器是怎么背创建出来的？
  - 2. 什么是双亲委派机制？为什么要有这种机制？
  - 3. Class实例和类加载器究竟是在Java Heap中，还是在方法区中？
  - 4. 为何要有线程上下文类加载器

### Java最大栈深度有多大
- 相关文章：
  - [Java最大栈深度有多大](https://www.itzhai.com/jvm/how-stack-frame-can-a-thread-hold.html)
- 关键词：`堆栈`
- 相关问题：
  - 1. Java最大栈深度多大
  - 2. 程序中如何调优

### Java代码编译方式和JVM三种执行模式
- 相关文章：
  - [Java代码编译方式和JVM三种执行模式](https://www.itzhai.com/jvm/java-code-compilation-mode-and-jvm-3-execution-modes.html)
- 关键词：`JIT` `javac`
- 相关问题：
  - 1. Java代码编译方式有哪些？
  - 2. JVM执行方式有哪些？

### JVM是如何进行方法调用的
- 相关文章：
  - [JVM是如何进行方法调用的](https://www.itzhai.com/jvm/how-the-jvm-makes-method-calls.html)
- 关键词：`静态分派` `动态分派`
- 相关问题：
  - 1. JVM里面是如何进行方法调用的？
  - 2. 什么是静态分派？
  - 3. 什么是动态分派？
  - 4. 怎么保证动态分派的执行效率？
  - 5. 重写和重载的执行原理？

### javac编译器
- 相关文章：
  - [10分钟教你如何hack掉Java编译器](https://www.itzhai.com/jvm/java-code-from-compilation-to-execution.html)
- 关键词：`编译流程` `javac` `JIT` `注解处理器`
- 相关问题：
  - 1. 编译器一般编译流程
  - 2. javac的编译流程是怎样的
  - 3. 如何hack掉Java编译器
  - 4. 运行时DI和编译期DI的区别

### Java泛型
- 相关文章：
  - [深入探索Java泛型的本质](https://www.itzhai.com/jvm/exploring-the-nature-of-java-generics.html)
- 关键词：`泛型`
- 相关问题：
  - 1. 为什么需要泛型
  - 2. Java代码在编译后是如何保存泛型信息的
  - 3. Java泛型与C++、Python中的有何区别
  - 4. 如何动态获取泛型类型

### JIT编译器
- 相关文章：
  - [Java界的性能优化高手](https://www.itzhai.com/jvm/what-exactly-does-the-java-compiler-do.html)
  - 关键词：`编译器` `解释器` `JIT`
  - 相关问题：
    - 1. javac做了什么优化
    - 2. Java后端编译器的发展史
    - 3. JIT是如何工作的
    - 4. 效率与质量的衡量

!> 在整理这个专题的时候，出了一个高效学习的介绍文章，这里也推荐给大家：[碎片化知识盛行，学东西如何做到过目不忘](https://www.itzhai.com/jvm/efficient-learning-and-memory-method.html)
