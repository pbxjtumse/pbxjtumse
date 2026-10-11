<div align="center">

# 👋 Hi, I'm Pang Bo

### Backend Engineer · Distributed Systems · AI Engineering

[![GitHub](https://img.shields.io/badge/GitHub-pbxjtumse-181717?logo=github&logoColor=white)](https://github.com/pbxjtumse)
[![Email](https://img.shields.io/badge/Email-pbxjtumse%40outlook.com-0078D4?logo=microsoftoutlook&logoColor=white)](mailto:pbxjtumse@outlook.com)

<br>

<a href="#english-profile">
  <img src="https://img.shields.io/badge/English-0969DA?style=for-the-badge">
</a>
<a href="#chinese-profile">
  <img src="https://img.shields.io/badge/简体中文-0969DA?style=for-the-badge">
</a>

</div>

---

<a id="english-profile"></a>

# 🇬🇧 English Profile

## 👨‍💻 About Me

I am a backend engineer focused on distributed systems, high-concurrency processing, reusable infrastructure components, and production-oriented AI engineering.

My primary engineering stack is **Java / Spring Boot**. I am currently building a reusable Java infrastructure component ecosystem and using it to study how retry, idempotency, transactions, messaging, distributed coordination, storage routing, governance, and observability should work together in real business systems.

I am also gradually extending this experience into **Python-based AI engineering**, especially LLM applications, RAG, Agent workflows, tool calling, MCP, durable execution, evaluation, and AI observability.

---

## 🚀 Current Focus

```text
Java Infrastructure Engineering
├── Foundation & Common Runtime
├── Concurrency & Async Execution
├── Retry & Reliable Task
├── Transaction & Idempotency
├── Distributed Lock & Fencing Token
├── Messaging
├── Cache
├── Governance
├── Observability
├── Relational Access
└── Storage Routing

AI Engineering
├── LLM Applications
├── RAG & Knowledge Systems
├── Agent Workflows
├── LangChain / LangGraph
├── Tool Calling / MCP
├── Memory & State
├── Evaluation / Guardrails
└── AI Observability

Cloud Native
├── Kubernetes / Docker
├── Kafka / Pulsar / RocketMQ
├── Redis / MySQL / PostgreSQL
├── Elasticsearch
├── Flink Kubernetes Operator
├── GitOps / Argo CD
└── Prometheus / Grafana / OpenTelemetry
```

---

## 🧩 Featured Project — Iron Components Java

### [iron-components-java](https://github.com/pbxjtumse/iron-components-java)

A reusable Java / Spring Boot technical component ecosystem for distributed business systems.

The project does **not** try to reimplement Redis, Kafka, Pulsar, RocketMQ, OpenTelemetry, Resilience4j, ShardingSphere, or Spring Transaction. Instead, it builds a stable engineering layer above mature infrastructure:

```text
Business Code
    ↓
Stable API / Starter
    ↓
Core Orchestration
    ↓
SPI / Integration
    ↓
Provider
    ↓
Mature Infrastructure
```

The goal is to reduce duplicated infrastructure code and make technical capabilities composable, observable, replaceable, and easier to evolve.

[![Repository](https://img.shields.io/badge/GitHub-iron--components--java-181717?logo=github&logoColor=white)](https://github.com/pbxjtumse/iron-components-java)
[![Components](https://img.shields.io/badge/Source-components-0969DA?logo=github&logoColor=white)](https://github.com/pbxjtumse/iron-components-java/tree/master/component)

### Current Component Map

```text
Iron Components Java
├── Foundation
├── Concurrency
├── Retry
├── Reliable Task
├── Transaction
├── Idempotent
├── Distributed Lock
├── Message
├── Cache
├── Governance
├── Observability
├── Relational Access
└── Storage Routing
```

### What the project currently explores

* **Foundation** — time, IDs, serialization, context propagation, reflection, resources, reusable low-level abstractions
* **Concurrency** — thread-pool governance, async tasks, timeout, cancellation, fallback, lifecycle and metrics
* **Retry** — explicit, bounded, observable short-cycle retries with classification and backoff
* **Reliable Task** — persistent tasks, CAS claiming, lease, recovery scanning and cross-process execution recovery
* **Transaction** — unified local transaction execution abstraction on top of Spring transactions
* **Idempotency** — owner/version state machine, replay, recovery takeover, Redis/JDBC persistence and route-aware storage
* **Distributed Lock** — Redis / Redisson providers, watchdog, owner token and fencing-token protection
* **Message** — unified Kafka / Pulsar / RocketMQ message model, send/consume lifecycle, reliability and ACK/redelivery semantics
* **Cache** — Caffeine + Redis multi-level cache, cache policies, load protection, invalidation events and observability
* **Governance** — timeout, retry, rate limiting, circuit breaking, bulkhead isolation and Resilience4j integration
* **Observability** — tracing abstraction, MDC propagation, OpenTelemetry adapter and Spring integration
* **Relational Access** — reusable JDBC/relational execution boundary, connection handling, exception translation and transaction reuse
* **Storage Routing** — direct datasource routing plus ShardingSphere-JDBC / Proxy integration for sharding-oriented access

### Engineering Principles

```text
Stable API
+ Explicit execution semantics
+ Clear module boundaries
+ Replaceable providers
+ Composition over duplication
+ Transaction-aware integration
+ Observable runtime behavior
+ Code-first documentation
```

---

## 🔗 Capability Composition

The project is designed around combinations rather than isolated utilities.

```text
Reliable Consume
Message
  + Idempotent
  + Transaction
  + Retry
  + Observability

Reliable Send
Message
  + Retry
  + Reliable Task / Outbox
  + Transaction
  + Observability

Consistent Data Access
Storage Routing
  + Relational Access
  + Transaction
  + Idempotent

Distributed Coordination
Distributed Lock
  + Fencing Token
  + Relational Access

Async Governance
Concurrency
  + Governance
  + Observability
```

---

## 🤖 AI Engineering Direction

My next engineering direction is to reuse the same reliability mindset for AI-native systems.

Rather than treating AI applications as prompt wrappers, I am interested in production concerns such as:

* Model provider abstraction
* Prompt and tool lifecycle
* LangGraph-based workflow orchestration
* Agent runtime and state management
* Short-term / long-term memory
* RAG and retrieval pipelines
* Durable execution and recovery
* Human-in-the-loop workflows
* Evaluation and guardrails
* Trace, token, latency and cost observability
* Integration between AI runtimes and traditional backend systems

Python will be the primary language for this part of the stack, while Java remains an important integration and enterprise backend runtime.

---

## ☁️ Cloud-Native Lab

I also maintain a personal environment for architecture validation, middleware integration, troubleshooting and performance experiments.

Main technologies include:

* Kubernetes / Docker
* Kafka / Pulsar / RocketMQ
* Redis / MySQL / PostgreSQL / MongoDB
* Elasticsearch / Kibana / ECK
* Flink Kubernetes Operator
* Longhorn / MinIO
* Harbor / GitLab
* Argo CD
* Prometheus / Grafana
* OpenTelemetry

---

## 🧠 Engineering Interests

```text
Distributed Systems
        +
Reliable Execution
        +
Enterprise Engineering
        +
Cloud Native
        +
AI Agent Runtime
        +
Production AI
```

I am especially interested in systems where correctness and reliability depend on more than a successful API call:

**idempotency, transaction boundaries, retries, durable recovery, distributed coordination, messaging semantics, state management, observability and operational governance.**

---

## 📫 Contact

* GitHub: [@pbxjtumse](https://github.com/pbxjtumse)
* Email: `pbxjtumse@outlook.com`
* WeChat: `pbdwxin`

<div align="right">

[⬆ Back to top](#)

</div>

---

<a id="chinese-profile"></a>

# 🇨🇳 中文介绍

## 👨‍💻 关于我

后端开发工程师，主要关注 **分布式系统、高并发处理、可复用技术组件以及面向生产环境的 AI 工程化**。

当前主要技术积累集中在 **Java / Spring Boot**。正在持续建设一套可复用的 Java 技术组件体系，并以此研究 Retry、幂等、事务、消息、分布式协调、存储路由、治理和可观测性如何在真实业务系统中组合工作。

同时也在逐步把这些传统后端工程经验迁移到 **Python AI 工程体系**，重点关注 LLM、RAG、Agent Workflow、Tool Calling、MCP、Durable Execution、Evaluation 以及 AI Observability。

---

## 🚀 当前关注方向

```text
Java 技术组件体系
├── Foundation / 基础运行时
├── Concurrency / 异步执行
├── Retry / Reliable Task
├── Transaction / Idempotent
├── Distributed Lock / Fencing Token
├── Message
├── Cache
├── Governance
├── Observability
├── Relational Access
└── Storage Routing

AI 工程
├── LLM Application
├── RAG / Knowledge System
├── Agent Workflow
├── LangChain / LangGraph
├── Tool Calling / MCP
├── Memory / State
├── Evaluation / Guardrail
└── AI Observability

云原生
├── Kubernetes / Docker
├── Kafka / Pulsar / RocketMQ
├── Redis / MySQL / PostgreSQL
├── Elasticsearch
├── Flink Kubernetes Operator
├── GitOps / Argo CD
└── Prometheus / Grafana / OpenTelemetry
```

---

## 🧩 代表项目 — Iron Components Java

### [iron-components-java](https://github.com/pbxjtumse/iron-components-java)

一套面向 Java / Spring Boot 分布式业务系统的可复用技术组件体系。

项目不会重新实现 Redis、Kafka、Pulsar、RocketMQ、OpenTelemetry、Resilience4j、ShardingSphere 或 Spring Transaction，而是在这些成熟基础设施之上建立一层更稳定、更贴近业务系统的工程抽象：

```text
业务代码
    ↓
稳定 API / Starter
    ↓
Core 编排
    ↓
SPI / Integration
    ↓
Provider
    ↓
成熟基础设施
```

目标是减少重复建设，让技术能力具备更清晰的边界，并能够组合、替换、观测和持续演进。

[![Repository](https://img.shields.io/badge/GitHub-iron--components--java-181717?logo=github&logoColor=white)](https://github.com/pbxjtumse/iron-components-java)
[![Components](https://img.shields.io/badge/Source-components-0969DA?logo=github&logoColor=white)](https://github.com/pbxjtumse/iron-components-java/tree/master/component)

### 当前组件全景

```text
Iron Components Java
├── Foundation
├── Concurrency
├── Retry
├── Reliable Task
├── Transaction
├── Idempotent
├── Distributed Lock
├── Message
├── Cache
├── Governance
├── Observability
├── Relational Access
└── Storage Routing
```

### 当前重点能力

* **Foundation**：时间、ID、序列化、上下文传播、反射、资源等底层公共能力
* **Concurrency**：线程池治理、异步任务、超时、取消、fallback、生命周期和指标
* **Retry**：显式、有限、可观测的短周期重试
* **Reliable Task**：持久化任务、CAS 抢占、Lease、扫描兜底以及跨进程恢复
* **Transaction**：基于 Spring Transaction 的统一本地事务执行抽象
* **Idempotent**：owner/version 状态机、结果回放、Recovery、Redis/JDBC 存储和路由感知
* **Distributed Lock**：Redis / Redisson、Watchdog、Owner Token、Fencing Token
* **Message**：Kafka / Pulsar / RocketMQ 统一消息模型、发送消费生命周期以及 ACK / Redelivery 语义
* **Cache**：Caffeine + Redis 多级缓存、缓存策略、加载保护、失效事件和可观测性
* **Governance**：超时、重试、限流、熔断、隔离和 Resilience4j 集成
* **Observability**：Trace 抽象、MDC 上下文、OpenTelemetry Adapter 和 Spring 集成
* **Relational Access**：统一关系型访问边界、连接管理、异常转换以及事务连接复用
* **Storage Routing**：Direct DataSource 路由，以及 ShardingSphere-JDBC / Proxy 集成

### 设计原则

```text
稳定 API
+ 显式执行语义
+ 清晰模块边界
+ Provider 可替换
+ 能力组合而不是重复实现
+ 事务感知
+ 可观测
+ 代码优先文档
```

---

## 🔗 技术能力组合

真正有价值的不是某一个孤立组件，而是组件之间形成完整执行链路。

```text
可靠消费
Message
  + Idempotent
  + Transaction
  + Retry
  + Observability

可靠发送
Message
  + Retry
  + Reliable Task / Outbox
  + Transaction
  + Observability

一致性数据访问
Storage Routing
  + Relational Access
  + Transaction
  + Idempotent

分布式协调
Distributed Lock
  + Fencing Token
  + Relational Access

异步治理
Concurrency
  + Governance
  + Observability
```

---

## 🤖 AI 工程方向

下一阶段希望把同样的可靠性思路带入 AI Native Application。

相比只完成 Prompt Demo 或简单模型 API 调用，我更关注：

* Model Provider 抽象
* Prompt / Tool 生命周期
* 基于 LangGraph 的 Workflow 编排
* Agent Runtime 与状态管理
* 短期 / 长期 Memory
* RAG 与 Retrieval Pipeline
* Durable Execution / Recovery
* Human-in-the-loop
* Evaluation / Guardrail
* Trace / Token / Latency / Cost Observability
* AI Runtime 与传统业务系统的集成

这一部分会优先使用 Python；Java 继续承担企业级后端以及与 AI Runtime 的集成职责。

---

## ☁️ 云原生实验环境

用于中间件部署、架构验证、故障排查以及性能实验：

* Kubernetes / Docker
* Kafka / Pulsar / RocketMQ
* Redis / MySQL / PostgreSQL / MongoDB
* Elasticsearch / Kibana / ECK
* Flink Kubernetes Operator
* Longhorn / MinIO
* Harbor / GitLab
* Argo CD
* Prometheus / Grafana
* OpenTelemetry

---

## 🧠 长期关注

```text
Distributed Systems
        +
Reliable Execution
        +
Enterprise Engineering
        +
Cloud Native
        +
AI Agent Runtime
        +
Production AI
```

尤其关注那些不能仅靠“一次 API 调用成功”解决的问题：

**幂等、事务边界、重试、持久化恢复、分布式协调、消息语义、状态管理、可观测性以及运行时治理。**

---

## 📫 联系方式

* GitHub：[@pbxjtumse](https://github.com/pbxjtumse)
* Email：`pbxjtumse@outlook.com`
* WeChat：`pbdwxin`

<div align="right">

[⬆ 返回顶部](#)

</div>

---

<div align="center">

### Build reliable systems · Engineer production AI

构建可靠系统 · 打造生产级 AI 工程

</div>
