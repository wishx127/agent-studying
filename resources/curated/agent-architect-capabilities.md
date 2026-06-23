# Agent 架构师能力扩展清单

> 2026-06-23 通过三通道并发搜索整理
> 来源：web_search + agent-reach（知乎/V2EX/B站）+ code_search

---

## 搜索发现的新增知识节点（19 个）

| 编号 | 节点名 | 归属领域 | 来源 |
|------|--------|---------|------|
| A.26 | Context Engineering | Agent 核心 | V2EX + Anthropic 指南 |
| A.27 | Agent 评估体系 | Agent 核心 | web_search + Anthropic Eval 指南 |
| A.28 | Agent 测试策略 | Agent 核心 | web_search |
| A.29 | Self-Reflection 与 Agentic RAG | Agent 核心 | 知乎「5种 Agent 模式」 |
| A.30 | MCP/A2A 协议 | Agent 核心 | MCP/A2A 官方规范 |
| A.31 | ADLC（Agent 开发生命周期） | Agent 核心 | web_search |
| A.32 | Agent Skills 架构 | Agent 核心 | 知乎「Agent/Skills/Teams」 |
| B.18 | Guardrails 安全防护系统 | 企业级后端 | web_search |
| B.19 | Model Gateway（模型网关） | 企业级后端 | web_search |
| B.20 | 企业集成层设计 | 企业级后端 | web_search |
| C.17 | 语义缓存 | 基础设施 | web_search |
| C.18 | 成本归因与 Token 计费 | 基础设施 | web_search |
| D.10 | Agent-Native CI/CD | 生产运维 | web_search |
| E.9 | Agent 流式输出 UX 设计 | 前后端协同 | web_search |
| F.8 | Prompt 版本管理 | 工程效能 | web_search |
| F.9 | 可观测性平台 | 工程效能 | web_search |

---

## 面试高频 Top 20（来自搜索）

1. 什么是 Agent？与大模型有什么本质不同？
2. ReAct、Plan-and-Execute、Reflection 三种范式的核心区别和选型？
3. 如何设计 Agent 的记忆系统（短期/长期）？
4. 如何选择和设计 RAG 的 chunk 策略和检索方案？
5. Multi-Agent 系统有哪些编排模式？生产中最常用哪个？
6. MCP 和 A2A 协议分别解决什么问题？
7. 如何评估 Agent 的质量？有哪些关键指标？
8. 如何防御 Prompt Injection？多层防御模型是什么？
9. 如何控制 Agent 的 token 成本？
10. 企业级 Agent 系统的整体架构设计？
11. LangGraph 的 StateGraph 如何工作？Checkpointing 有什么用？
12. 如何做 Agent 的 CI/CD？与传统 CI/CD 有什么区别？
13. Agent 的可观测性包含哪些支柱？
14. 如何做 Agent 的 A/B 测试和灰度发布？
15. Function Calling 的实现原理和各家差异？
16. 如何处理 Agent 工具调用失败？
17. Embedding 模型选型的方法论和常见陷阱？
18. Agent 的多租户隔离怎么做？
19. 从 Demo 到生产，Agent 系统需要解决哪些问题？
20. 如何设计 Agent 的 Human-in-the-Loop 机制？

---

## 推荐学习资源

| 类别 | 资源 | 说明 |
|------|------|------|
| 官方指南 | [Anthropic: Building Effective AI Agents](https://resources.anthropic.com/) | 架构模式和实现框架 |
| 官方指南 | [Anthropic: Demystifying Evals for AI Agents](https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents) | Agent 评估方法论 |
| 官方指南 | [Anthropic: Effective Context Engineering](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents) | 上下文工程最佳实践 |
| 架构参考 | [Google Cloud: Choose a Design Pattern for Agentic AI](https://docs.cloud.google.com/architecture/choose-design-pattern-agentic-ai-system) | 设计模式选择指南 |
| 架构参考 | [Microsoft: AI Agent Orchestration Patterns](https://learn.microsoft.com/en-us/azure/architecture/ai-ml/guide/ai-agent-design-patterns) | 多 Agent 编排模式 |
| 开源参考 | [Microsoft: Multi-Agent Reference Architecture](https://github.com/microsoft/multi-agent-reference-architecture) | 多 Agent 参考架构 |
| 面试题 | [JavaGuide: AI 系统设计面试题](https://javaguide.cn/ai/interview-questions/ai-interview-guide.html) | 中文面试题大全 |
| 面试题 | [ai-agent-interview-guide](https://github.com/bcefghj/ai-agent-interview-guide) | 企业级 Agent 面试问答集 |
| 框架文档 | [LangGraph Docs](https://docs.langchain.com/oss/python/langgraph/) | LangGraph 官方文档 |
| 框架文档 | [Context Engineering Handbook](https://github.com/ypollak2/context-engineering-handbook) | 35 个实战模式 |
| 协议规范 | [MCP Specification](https://modelcontextprotocol.io/) | Model Context Protocol |
| 协议规范 | [A2A Protocol](https://a2a-protocol.org/) | Agent-to-Agent Protocol |
