# Session 记录 - 2026-07-15（Session 2）

## Session 概览

- **日期**: 2026-07-15
- **阶段**: Phase 1 — 全景扫描
- **主题**: B.14 认证鉴权（JWT/OAuth2/RBAC）

---

## 学习内容

### B.14 认证鉴权

**学生初始理解**:

- 认证是确认“你是谁”，鉴权是确认“你可以做什么”
- JWT 可以帮助认证用户身份
- 对 RBAC 不熟悉

**讲解方式**:

- 区分认证（Authentication）和鉴权（Authorization）
- 说明 JWT 是 Token 格式，通常通过签名保护 Header/Payload 的完整性；JWT 不等于加密，也不直接解决密钥分发
- 讲解 RBAC 的用户 → 角色 → 权限关系
- 讲解 OAuth2 四个角色：Resource Owner、Client、Authorization Server、Resource Server
- 对比 Authorization Code + PKCE、Client Credentials，以及旧式 Implicit/Password 模式
- 对比 JWT 与 Opaque Token：本地验签 vs Introspection/共享存储查询

**理解检验**:

- 能正确判断修改 JWT Payload 后签名验证失败
- 能识别 Editor 是角色，`article:update` 是权限
- 能将用户授权场景映射到 Authorization Code，将服务间调用映射到 Client Credentials
- 能判断合法 JWT 代表认证通过，但缺少 admin 权限时鉴权失败并拒绝请求

**达成掌握程度**: L1

---

## 本次 Session 总结

### 达成的掌握程度

| 领域 | 知识点 | 深度 | 状态 |
|------|--------|------|------|
| B. 企业级后端 | B.14 认证鉴权 | L1 | 🟡 学习中 |

### 知识缺口

- 尚未进入 L2 的完整认证鉴权方案设计
- 尚未深入 Token 刷新、撤销、轮换、CSRF 与 Cookie 存储策略

### 下次 Session 建议

- **优先学习**: B.15 API 安全
- **强化**: 401（认证失败）与 403（权限不足）的错误响应边界
