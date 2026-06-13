# 🎉 AI协作开发前期规范 v3.1.0

> **AI Collaborative Development Preflight — Runtime Execution Engine**

---

## 🔧 v3.1.0 更新内容

### 模拟对话强化（Simulated Dialogue Hardening）

- **STEPS → PHASES with loop gates**: 12步线性模型升级为11阶段循环门控
- **每阶段强制覆盖清单**: Direction(6项) / Feature(10项) / Engineering(12项)
- **问题格式V2**: 每个选项必须包含优缺点、术语解释、"你也可以提出新方案"邀请
- **【STATE】输出**: 每轮回复开头声明当前状态
- **完整性门控**: 18项检查清单，任何 ⚠️/❌ 触发阶段重循环
- **新方案处理**: 用户提新想法 → PAUSE → 验证阶段完整性 → 必要时重循环
- **LIGHT→FULL 升级路径**: 小改动需要架构支持时自动升级到 FULL MODE Phase 1
- **详细回滚规范**: 6步变更管理 + 受影响决策表 + 模块影响映射
- **紧凑【ROUND OUTPUT】格式**: 摘要 + 决策表 + 风险合并输出

---

## 🚀 v3.0.0 核心特性

### 可执行运行时引擎
- SKILL.md 重写为运行时执行引擎，非参考文档
- **FULL MODE** (11阶段) 和 **LIGHT MODE** (6阶段)
- 状态机: INIT → UNDERSTAND → QUESTION → LOCK → SPEC → CONFIRM → READY
- 硬约束: 早期阶段只能输出 A/B/C/D/E 选项
- 强制决策锁定表输出
- **绝对禁止**: SPEC 批准前不得输出任何代码

---

## 📦 安装

1. 下载 `ai-preflight-skill.zip`
2. 解压到 Codex skills 目录: `C:\Users\<用户名>\.codex\skills\`
3. 重启 Codex

---

## 📥 Assets

| 文件 | 说明 |
|------|------|
| `ai-preflight-skill.zip` | Codex Skill Plugin 完整包 |