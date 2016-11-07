# 系统架构知识图谱

## PHP 
  * 配置：php.ini / fpm配置
  * 代码规范 PSR
  * PHP面向对象
  * SPL
  * 依赖管理：Composer
    * Library的编写与发布
  * PHPUnit
  * PHP框架
    * symfony / symfony components
    * laravel
    * silex
    * phalcon
  * Swoole
  * zephir
  * 模板引擎
    * 模板引擎原理
    * Twig
  * 错误异常处理
  * 调试: Xdebug
  * 部署
    * Deployer: http://deployer.org/
    * nginx / apache
  * 序列化/反序列化
  * 缓存技术
  * PHPDoc
  * PHP运行的生命周期
  * PHP命令行程序编写
  * 优秀PHP项目源码解读
    * [Drupal](https://www.drupal.org/)
    * [October](https://github.com/octobercms/october)

## 第二语言Go 

## 数据库

  * MySQL
    * Innodb引擎
    * Binglog
    * 备份策略
    * 性能调优
    * 锁
    * 事务
    * 监控
    * MySQL Replication 
    * DRBD
    * MHA
    * 容量规划
  * Redis
    * 各种数据结构的使用场景
    * 复制
    * 事务
    * 集群
    * 配置优化

学习教材：

  * [高性能MySQL](https://book.douban.com/subject/23008813/)
  * [MySQL性能调优与架构设计](https://book.douban.com/subject/3729677/)
  * [Redis实战](https://book.douban.com/subject/26612779/)

## Web开发安全
  * XSS
  * CSRF
  * SQL Injection
  * 会话劫持
  * 加密算法
  * 签名算法
  * 服务器入侵检测
  * 开发安全流程构建

学习教材：

  * [《白帽子讲Web安全》](https://www.amazon.cn/dp/B00LADBDG6/)

## 编程实践

  * 数据结构与算法
    * 算法复杂度计算
    * 常用数据结构
    * 实用算法
  * 面向对象设计
  * SOILD
  * 设计模式
  * 重构
  * 测试驱动开发
    * 单元测试
      * Mockery
    * 功能测试
    * 性能测试
  * 行为驱动开发
  * 持续集成

学习教材：

  * [算法（第4版）](https://book.douban.com/subject/19952400/)
  * [算法的乐趣](https://book.douban.com/subject/26351257/)
  * [面向对象分析与设计(第3版)](https://www.amazon.cn/dp/B01GE1UYAE)
  * [Head First设计模式(中文版)](https://www.amazon.cn/dp/B0011FBU34)
  * [重构:改善既有代码的设计](https://www.amazon.cn/dp/B011LPUB42/)
  * [企业应用架构模式](https://www.amazon.cn/dp/B003LBSRDM)

## 网络编程

  * 理论知识
    * OSI模型
    * TCP/UDP协议
    * DNS/RDNS
    * NAT
    * IP隧道
    * HTTP / HTTPS / HTTP2
    * WebSocket
    * MQTT
  * Linux内核网络参数
  * 基本TCP套接字编程
  * 基本UDP套接字编程
  * select / poll
  * POSIX信号量
  * IPC / 管道 / Posix消息队列
  * 共享内存
  * zeromq
  * 通讯协议设计

学习教材：

  * [计算机网络（第6版）](https://book.douban.com/subject/26176870/)
  * [UNIX网络编程 卷1：套接字联网API（第3版）](https://book.douban.com/subject/26434583/)
  * [UNIX网络编程 卷2：进程间通信（第2版）](https://book.douban.com/subject/26434599/)

## 运维

  * Linux命令
  * 防火墙配置：iptables
  * 自动化运维： Ansible
  * 监控：Zabbix
  * 日志收集 、分析
  * 容器技术：Docker

学习教材：

  * [Linux大棚命令百篇（上）](https://book.douban.com/subject/26849802/)
  * [Linux大棚命令百篇（下）](https://book.douban.com/subject/26849844/)
  * [Ansible自动化运维：技术与佳实践](https://book.douban.com/subject/26834737/)

## 大型网站架构技术

  * 高性能
    * 性能测试指标
    * 性能测试方法
      * Jmeter
    * 性能测试报告
    * 性能优化
      * 前端优化
      * 应用服务器优化
        * 缓存
          * 缓存的设计模式
          * Redis
        * 异步
          * Beanstalk
          * RabbitMQ
          * Kafka
        * 负载均衡
          * Nginx
          * LVS
          * Seesaw
          * Maglev
        * 代码优化：多线程、资源复用、数据结构算法优化
        * 存储性能优化
          * 固态硬盘
          * B + 数 vs LSM数
          * RAID vs HDFS
      * 优化分析工具
  * 高可用
    * 分层：应用层、服务层、数据层
    * 应用层
      * 无状态
      * 失效转移
      * Session集群
    * 服务层
      * 分级管理
      * 超时设置
      * 异步调用
      * 服务降级
      * 幂等性设计
    * 数据层
      * CAP理论
      * 数据备份
      * 失效转移
        * MHA
        * Linux Heartbeat
    * 软件质量保障
      * 代码控制
        * Git分支策略
        * Code Review
      * 自动化测试
      * 自动化发布
      * 灰度发布
    * 运行监控
  * 伸缩性
    * 伸缩性设计方法
      * 不同功能进行物理分离
      * 单一功能集群化
    * 应用服务器集群
      * HTTP重定向
      * DNS域名解析负载均衡
      * 反向代理负载均衡
      * IP负载均衡
      * 数据链路层负载均衡
      * 负载均衡算法
    * 分布式缓存集群
      * Sharding策略
      * 一致性Hash
    * 数据存储服务器集群
      * MySQL Master / Slave
      * NoSQL
  * 可扩展
    * 消息队列
    * 分布式服务
      * RPC
      * 服务注册、发现
      * 配置中心
    * 可扩展的数据结构
  * 安全架构
    * Web应用防火墙WAF
    * DDOS
    * 漏洞扫描
    * 信息加密技术
    * 信息过来及反垃圾
    * 风险控制

推荐书籍：

  * [大型网站技术架构](https://book.douban.com/subject/25723064/)
  * [分布式服务框架：原理与实践](https://book.douban.com/subject/26702824/)
  * [大型分布式网站架构：设计与实践](https://book.douban.com/subject/25972633/)

## 架构师软素质
  * 项目管理能力
  * 创新、学习能力
  * 沟通、解决问题能力
  * 设计美学
  * 用户体验
  * 商业逻辑
