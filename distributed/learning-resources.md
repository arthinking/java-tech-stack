# 分布式学习资源

## 在线资源

* :office: [Kafka官方文档](https://kafka.apache.org/documentation/)

### 消息队列之RabbitMQ

- 关键词：`高可用` `集群` `存储架构` `顺序消费` `延迟队列` `事务消息`
- 相关文章：
  - [消息队列那么多，为什么建议深入了解下RabbitMQ？](https://www.itzhai.com/articles/rabbitmq-advanced-tutorial.html)
- 相关问题：
  - 什么是AMQP？
  - 常见的交换机类型有哪些？
  - 如何实现消息的持久化？
  - RabbitMQ的连接复用有啥优势？
  - RabbitMQ的消息ACK机制是如何实现的？
  - RabbitMQ消息持久化机制性能如何？
  - 如何避免消费过载的问题？
  - 如何提高手动ACK签收的效率？
  - 什么时候需要让消息重回队列？
  - 如何保证消息的顺序消费？
  - 如何实现可靠的消息投递？

### 消息队列之RocketMQ

- 关键词：`高可用` `集群` `存储架构` `顺序消费` `延迟队列` `事务消息`
- 相关文章：
  - [高并发异步解耦利器：RocketMQ究竟强在哪里？](https://www.itzhai.com/articles/deep-understanding-of-rocketmq.html)
- 相关问题：
  - RocketMQ如何保证消息存储的可靠性？
  - RocketMQ如何保证消息队列服务的高可用？
  - 如何构建一个高可用的RocketMQ双主双从最小集群？
  - RocketMQ消息是如何存储的？
  - RocketMQ是如何保证存取消息的效率的？
  - 如何实现基于Message Key的高效查询？
  - 如何实现基于Message Id的高效查询？
  - RocketMQ的Topic在集群中是如何存储的？
  - Broker自动创建Topic会有什么问题？
  - RocketMQ如何保证消息投递的顺序性？
  - RocketMQ如何保证消息消费的顺序性？
  - 实现分布式事务的手段有哪些？
  - RocketMQ如何实现事务消息？
  - RocketMQ事务消息是如何存储的？

### 消息队列之Kafka

- 关键词：`Partition` `Controller` `Rebalance` `消息堆积` `延时队列` `重复消费` `offset` `ISR`
- 相关文章：
    - [Kafka必知必会18问：30+图带您看透Kafka](https://www.itzhai.com/articles/deep-understanding-of-kafka.html)
- 相关问题：
    - Kafka是如何存储和检索消息的？(log文件，index索引文件，timeindex索引文件)
    - Kafka是如何基于offset查找消息的？
    - Kafka有哪些日志清理策略？什么场景下会用到？
    - ISR是干嘛的？
    - Kafka总控制器是干嘛的？如何选举出来的？
    - Topic的最优Leader副本是如何选举出来的？
    - 什么时候会触发消费的Rebalace？Kafka中有哪些Rebalance策略？
    - Rebalance是如何工作的？
    - Kafka是如何保证数据可靠性的？
    - Kafka是如何保证数据一致性的？
    - 消费者是如何提交offset的？
    - 有哪些消费历史消息的方法？
    - Kafka为啥性能这么高？
    - Kafka如何避免重复消费？
    - Kafka如何处理消息堆积？
    - 如何保证消息顺序性？
    - Kafka如何实现消息传递保障？
    - Kafka有哪些关键的生产者和消费者参数？
  
### 分布式算法

- 关键词：`Raft`
- 相关文章：
  - [用动图讲解分布式 Raft](https://mp.weixin.qq.com/s/US12ux7osqH_L0CtQyw-9A)
- 相关问题：

## 书籍

* :book: 《从Paxos到Zookeeper : 分布式一致性原理与实践》
* :book: 《分布式系统 : 概念与设计》
* :book: 《面向模式的软件架构 卷4：分布式计算的模式语言》



