# maven-catalog

# Agent Scaffold Lite ( Agent 脚手架)

这是一个基于 Java 开发的轻量级 Agent 架构脚手架，采用成熟的领域驱动设计（DDD）分层架构。通过本脚手架，开发者可以一键生成标准化的微服务工程结构，快速投入到 AI 智能体或后端业务逻辑的开发中。
[Agent Scaffold Lite GitHub 仓库](https://github.com/caliu1/agent-scaffold-lite)

## 📁 目录结构

生成的项目将包含以下标准模块：

- **`xxx-api`**: 暴露给外部的 API 接口定义（Dubbo / Feign / 契约等）。
- **`xxx-app`**: 应用层，负责组合领域服务，编排业务用例。
- **`xxx-domain`**: 领域层，包含核心的领域模型、领域服务和仓储接口，隔离业务逻辑。
- **`xxx-infrastructure`**: 基础设施层，负责数据库交互、缓存、消息队列、外部 API（如 LLM 调用）的底层实现。
- **`xxx-trigger`**: 触发层，包含 HTTP Controller、RPC 接口实现、定时任务或 MQ 监听器。
- **`xxx-types`**: 公共类型定义层，存放全局常量、枚举、基础 Response 对象等。
