# Kafka 数据处理项目

本项目通过Python实现了Apache Kafka在数据流处理中的四种典型应用场景，展示了Kafka生产者和消费者的基础用法以及与MySQL数据库、JSON文件的集成能力。

## 项目概述

本项目包含四个独立模块，分别演示以下功能：
1. Kafka生产者-消费者基础通信
2. 从MySQL数据库实时同步数据
3. 读取并传输JSON文件数据
4. 分区消息处理与消费者组管理

通过本项目的实现，展示了以下技术能力：
- Kafka集群的基本配置与管理
- Python客户端（kafka-python）的熟练使用
- 关系型数据库与消息队列的集成
- 结构化数据（JSON）处理
- Kafka分区策略与消费者负载均衡

## 技术栈

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Kafka](https://img.shields.io/badge/Apache_Kafka-3.5.1-%23231F20)
![MySQL](https://img.shields.io/badge/MySQL-8.0-%234479A1)

- **核心组件**: Kafka, Zookeeper
- **编程语言**: Python 3.10+
- **数据库**: MySQL 8.0
- **关键依赖库**: 
  - `kafka-python` 
  - `pymysql`
  - `uuid`
  - `json`

## 功能模块

### 1. 基础生产者消费者
- 实现简单的消息生产/消费模式
- 验证Kafka基础消息传输机制
- 支持文本消息的实时传输

### 2. MySQL数据同步
- 从MySQL数据库读取结构化数据
- 实现数据库变更的实时事件流
- 使用定时查询模拟实时数据捕获

### 3. JSON文件处理
- 读取本地JSON文件并解析
- 实现结构化数据的序列化传输
- 验证复杂数据格式的完整传递

### 4. 分区与消费者组
- 创建双分区Kafka主题
- 生产者实现分区消息路由
- 两个消费者分别监听不同分区
- 演示消费者组的并行处理能力
