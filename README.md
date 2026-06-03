# Tiny Ragent AI

## tiny parts

- 删除前端项目
- 删除 MCP 模块
- 减少模型服务提供商（仅保留硅基流动、阿里云百炼）

## core parts

### 多路并行检索引擎架构

```
检索配置 SearchChannelProperties
检索通道类型枚举 SearchChannelType
```

### 模型路由与高容错机制

```
模型路由执行器 ModelRoutingExecutor
向量服务路由 RoutingEmbeddingService
Rerank服务路由 RoutingRerankService

模型配置属性类 AIModelProperties
```

### 异步场景的全链路追踪

```text
采集切面 RagTraceAspect
```

### 分布式排队与限流推送

```text
queue_claim_atomic.lua
```