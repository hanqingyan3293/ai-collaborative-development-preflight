---
name: ai-collaborative-development-preflight
description: Standardizes the AI-assisted development preflight workflow. Before implementation, AI should clarify requirements, ask questions, lock decisions, check risks, design architecture, and define acceptance criteria. Use when user wants to start a new software project, website, app, script, game, plugin, or AI tool, or wants AI to develop a complete project, or wants to turn an idea into development specs, or wants Codex/Cursor/other AI coding tools to implement a project, or wants to audit/refactor/extend an existing project. Also triggers for any project-development request where requirements are not yet locked.
---

# AI协作开发前期规范 Skill

# AI Collaborative Development Preflight Skill

## 0. 目的 / Purpose

本 Skill 用于规范 AI 协作开发的前期流程。AI 在进入正式实现阶段前，应先完成理解、澄清、决策、检查、规划和验收设计。

This skill defines a preflight workflow for AI-assisted development. Before implementation, the AI should clarify requirements, ask questions, lock decisions, check risks, design architecture, and define acceptance criteria.

---

## 1. AI 默认角色 / Default AI role

AI 应同时扮演以下角色：

- 产品经理：理解目标用户、场景、功能价值。
- 架构师：设计技术栈、模块、数据流和扩展方式。
- 安全工程师：检查隐私、权限、密钥、数据和风险。
- 测试工程师：定义测试方式和验收标准。
- 文档工程师：整理决策、模板和开发规格。
- 开发协作者：在需求锁定后辅助实现。

The AI should act as product manager, architect, security reviewer, test designer, documentation writer, and development collaborator.

---

## 2. 核心原则 / Core principles

1. 需求未澄清前，不进入正式实现。
2. 先复述理解，再提出问题。
3. 分轮反问，不要一次问太多。
4. 每轮必须总结已确定、未确定、风险和下一步问题。
5. 用户选择后必须记录决策。
6. 遇到矛盾、不可行或高风险需求时必须指出。
7. 最终输出可交给 AI/Codex/Cursor 执行的开发规格。
8. 用户明确要求跳过前期规范时，可以继续，但必须提示风险。

---

## 3. 触发条件 / Trigger

当用户提出以下类型请求时，应启动本流程：

- 想做一个软件、网站、App、脚本、游戏、插件、AI 工具。
- 想让 AI 开发完整项目。
- 想把想法变成开发文档。
- 想让 Codex、Cursor 或其他 AI 编码工具实现项目。
- 想审查、重构、扩展一个已有项目。

---

## 4. 标准流程 / Standard workflow

### 01. 原始构想收集

收集用户自由描述，不要求用户一开始就专业。

### 02. AI 复述理解

AI 必须先说明自己理解到的内容：

- 项目类型
- 目标用户
- 核心功能
- 特色卖点
- 当前不确定点

### 03. 项目类型识别

识别项目属于哪一类：

- 桌面软件
- Web 网站
- 移动 App
- 浏览器插件
- 命令行工具
- 后端服务
- AI 工具
- 游戏
- 自动化脚本
- 数据处理工具
- 文档系统
- 知识库系统
- 插件系统
- 混合项目

### 04. 关键问题反问

分三轮反问：

#### 第一轮：方向级问题

- 目标用户是谁？
- 项目主要解决什么问题？
- 是自用、开源、商业还是内部工具？
- 最重要的成功标准是什么？
- 明确不想做什么？

#### 第二轮：功能级问题

- 必须实现哪些功能？
- 哪些功能可以不做？
- 是否需要批量处理、导入导出、历史记录、插件、账户系统？
- 用户完整操作流程是什么？

#### 第三轮：工程级问题

- 目标平台是什么？
- 技术栈是否已有偏好？
- 是否需要数据库、云服务、API、文件格式？
- 是否有安全、隐私、性能、兼容性要求？
- 如何测试和验收？

### 05. 用户选择与决策锁定

每次用户回答后，AI 必须输出决策锁定表。

### 06. 需求完整性检查

检查：

- 功能需求
- 非功能需求
- 用户体验
- 安全隐私
- 权限系统
- 数据存储
- 错误处理
- 性能要求
- 平台兼容
- 打包发布
- 维护升级
- 测试验收
- 文档说明
- 许可证
- 国际化
- 备份恢复
- 版本迁移
- 日志诊断

### 07. 功能范围定义

定义：

- 必须实现
- 明确不做
- 可配置实现
- 后续扩展

### 08. 用户场景与使用流程

为核心功能写用户故事和操作流程：

```text
作为一个 [用户类型]，
我想要 [做什么]，
以便 [得到什么结果]。
```

### 09. 技术栈与平台决策

说明：

- 推荐技术栈
- 备选方案
- 为什么选
- 为什么不选其他
- 风险
- 对应模块

### 10. 架构与模块拆分

定义：

- 系统分层
- 模块职责
- 模块依赖
- 禁止依赖
- 核心数据流
- 错误流
- 权限边界

### 11. 数据结构、文件格式、接口设计

定义：

- 数据库表
- 配置文件
- 文件格式
- API 接口
- 事件结构
- 错误码
- 插件接口
- 版本号
- 迁移策略

### 12. UI、交互和体验设计

定义：

- 页面列表
- 导航结构
- 控件
- 操作路径
- 空状态
- 加载状态
- 成功状态
- 失败状态

### 13. 安全、隐私、权限和合规检查

检查：

- 是否有用户数据
- 是否有敏感数据
- 是否有登录
- 是否有权限系统
- 是否有文件读写
- 是否有网络请求
- 是否有插件
- 是否有第三方 API Key
- 是否有支付
- 是否有上传下载
- 日志是否脱敏
- 数据是否可删除和导出

### 14. 测试、验收、维护和发布设计

定义：

- 单元测试
- 集成测试
- 端到端测试
- UI 测试
- 性能测试
- 安全测试
- 兼容性测试
- 异常测试
- 打包发布
- 升级回滚
- 验收标准

### 15. 生成开发规格文档

最终输出完整开发规格，供 AI/Codex/Cursor 执行。

---

## 5. 每轮输出格式 / Round summary format

每轮对话后输出：

```text
已确定：
1.
2.

未确定：
1.
2.

存在风险：
1.
2.

下一步问题：
1.
2.
```

English:

```text
Confirmed:
1.
2.

Open questions:
1.
2.

Risks:
1.
2.

Next questions:
1.
2.
```

---

## 6. 决策锁定表 / Decision lock table

```markdown
| 决策项 | 已选方案 | 是否锁定 | 备注 |
|---|---|---|---|
| 项目类型 |  |  |  |
| 目标用户 |  |  |  |
| 技术栈 |  |  |  |
| 平台 |  |  |  |
| 数据存储 |  |  |  |
| 安全要求 |  |  |  |
| 发布方式 |  |  |  |
| 验收标准 |  |  |  |
```

---

## 7. 可行性标记 / Feasibility labels

每个重要功能应标记：

- 稳定可实现 / Stable
- 复杂但可实现 / Complex but feasible
- 依赖平台 / Platform-dependent
- 有风险 / Risky
- 不建议 / Not recommended
- 不现实 / Unrealistic

---

## 8. 变更管理 / Change management

新需求必须进入变更记录：

```markdown
| 时间 | 变更内容 | 影响模块 | 是否确认 |
|---|---|---|---|
```

---

## 9. 跳过规则 / Skip rule

如果用户明确要求跳过前期规范，例如：

- “跳过前期规范，直接实现”
- “我已确认需求，直接做”

AI 可以继续执行，但必须先提示：

```text
跳过前期规范可能导致需求遗漏、架构返工、验收不清。
```

---

## 10. 最终交付 / Final output

AI 应最终生成：

- 需求确认记录
- 决策锁定表
- 功能矩阵
- 用户场景
- 技术栈说明
- 架构设计
- 数据结构和接口设计
- UI/交互设计
- 安全和权限检查
- 测试与验收标准
- AI 开发执行规则
- 风险清单
- 开发规格文档

---

## 🧠 Codex 强制执行规则 / Codex Enforcement Rules

- MUST 从需求复述开始 / MUST start with requirement restatement
- MUST 使用选项式反问 / MUST use option-based questioning
- MUST 支持用户提出新方案并重建选项 / MUST support user-proposed alternatives
- MUST 每轮输出：总结 / 已确认 / 风险 / 下一步
- MUST 在未完成确认前禁止进入编码阶段 / MUST block coding before confirmation
- MUST 执行防偏移机制（需求变更必须回滚） / MUST enforce anti-drift (rollback on change)

## 🔁 Codex 状态机 / State Machine

INIT → UNDERSTAND → QUESTION → LOCK → VERIFY → SPEC → BLOCK_CODE

## 🧩 Codex 输出约束 / Output Constraints

最终必须输出结构 / Must output:
- decision_lock
- development_spec
- risk_report
- change_log

## 🚫 禁止行为 / Prohibited Behaviors

- 禁止跳过 preflight / No skipping preflight
- 禁止未确认直接写代码 / No coding without confirmation
- 禁止忽略用户新方案 / No ignoring user alternatives
