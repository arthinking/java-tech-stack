# MySQL系列文章

### 底层架构

- 关键词：`undo log` `redo log ` `binlog` `MVCC` `双写缓冲区` `buffer pool` `change buffer` `log buffer` `聚集索引` `辅助索引` `B+树` `页结构` `行结构`
- [洞悉MySQL底层架构：游走在缓冲与磁盘之间](https://www.itzhai.com/database/insight-into-the-underlying-architecture-of-mysql-buffer-and-disk.html)
  - **整体架构：**InnoDB存储架构是怎样的
  - **工作原理：**查询语句的底层执行流程是怎样的 
  - **IO性能：**文件`IO操作`写磁盘有哪几种方式，有什么IO优化方式
  - **缓存：**`InnoDB缓存`(buffer pool, log buffer)的刷新方式有哪些
  - **缓存：**log buffer是在什么时候写入到磁盘的
  - **缓存：**为什么redo log prepare状态也要写磁盘？
  - **缓存：**脏页写盘一般发生在什么时候
  - **缓存：**为什么唯一索引的更新不可以借助change buffer
  - **缓存：**`log buffer`的日志刷盘控制参数`innodb_flush_log_at_trx_commit`对写性能有什么影响
  - **缓存：**buffer pool的LRU是如何实现的，为什么要这样实现
  - **表存储：**系统表空间的结构，MySQL InnoDB磁盘存储格式，各种`表空间`(系统表空间，独立表空间，通用表空间)的作用和优缺点是什么，`ibdata`、`ibd`、`frm`文件分别是干嘛的
  - **行字段存储：**底层页和行的存储格式
  - **行字段存储：**`varchar`，`null`底层是如何存储的，最大可用存储多大的长度
  - **行字段存储：**行记录太长了，一页存不下，该怎么存储？
  - **索引：**数据库`索引`的组织方式是怎样的，明白为什么要采用`B+树`，而不是哈希表、二叉树或者B树
  - **索引：**索引组织方式是怎样的，为什么`大字段`会影响表性能(查询性能，更新性能)
  - **索引：**`覆盖索引`、`联合索引`什么情况下会生效
  - **索引：**什么是`索引下推`，索引下推减少了哪方面的开销？
  - **索引：**`Change Buffer`对二级索引DML语句有什么优化
  - **数据完整性：**MySQL是如何保证数据完整性的，`redo log`、`undo log`和`buffer pool`数据完整性的关键作用分别是什么
  - **MVCC：**`MVCC`底层是怎么实现的，可重复读和读已提交是怎么实现的
  - 双写缓冲区有什么作用
  - Redo Log在一个事务中是在什么时候写入的？binlog和Redo Log有什么区别？


### 存储选型

- 相关文章：
  - [知不足而行. 数据库系统设计概述. 码哥字节.](https://mp.weixin.qq.com/s/HoSul-GjX6FmulY6ugdmgQ)
- 关键词：`发展史` `对象访问定位`
- 相关问题：
  - 1. 

### 索引

- 相关文章：
  - [深入理解 MySQL 索引底层原理](https://cloud.tencent.com/developer/article/1601047)
  - [数据库索引的知识点，你所需要了解的都在这儿了](https://mp.weixin.qq.com/s/MMUnZ-IEyR3RM-wyYsW4Vg)
- 关键词：`AVL树` `红黑树` `B树` `B+树`
- 相关问题：
