# AI协作开发前期规范 v3.1

> 让 AI 先想清楚，再写代码。  
> Make AI clarify, plan, and lock decisions before implementation.

《AI协作开发前期规范》是一套面向所有 AI 协作开发场景的开源流程规范。以 **Codex Skill Plugin** 形式交付——不是参考文档，而是 AI 运行时强制执行的规划引擎。

English: [README.en.md](./README.en.md)

## 项目定位

这是一个 **Runtime Execution Engine**，当 Codex 加载本 Skill 后，AI 在写代码前 **必须** 完成：

`理解 → 方向锁定 → 功能锁定 → 工程锁定 → 完整性检查 → 风险分析 → 架构设计 → 安全审查 → 测试验收 → SPEC 生成 → 用户确认`

全程 **11 个阶段**，每阶段有强制覆盖清单、出口条件和循环门控。用户提出新想法时自动暂停→验证→回滚。

## 快速安装

### 方式一：直接下载 Release（推荐）

1. 下载 [最新 Release 压缩包](https://github.com/hanqingyan3293/ai-collaborative-development-preflight/releases/latest)
2. 解压到 Codex skills 目录：
   ```
   C:\Users\<你的用户名>\.codex\skills\
   ```
3. 重启 Codex

解压后的目录结构：
```
.codex/skills/ai-collaborative-development-preflight/
├── .codex-plugin/plugin.json
├── skills/.../SKILL.md
├── agents/openai.yaml
├── README.md
├── LICENSE
└── CHANGELOG.md
```

### 方式二：Git Clone

```bash
git clone https://github.com/hanqingyan3293/ai-collaborative-development-preflight.git $CODEX_HOME/skills/ai-collaborative-development-preflight
```

## 快速使用

安装后，在 Codex 中输入以下任意语句即可触发：

```text
我想做一个项目，帮我先梳理需求
```

或直接描述项目构想，AI 会自动进入 FULL MODE 11 阶段流程。

## 核心流程

```
用户提出构想
     ↓
【复述理解】→ AI 复述确认
     ↓
╔══════════════════════════╗
║ 【提问 ⇄ 锁定】循环       ║
║  方向提问 → 锁定          ║
║  功能提问 → 锁定          ║
║  工程提问 → 锁定          ║
║  [完整性门控] ← 不通过则回退 ║
╚══════════════════════════╝
     ↓
【风险分析】→【架构设计】→【安全检查】→【测试验收】
     ↓
【SPEC 生成】→【用户确认】→ READY → 开始写代码
```

## 核心文件

| 文件 | 用途 |
|------|------|
| `.codex-plugin/plugin.json` | Codex 插件清单（Codex 识别入口） |
| `skills/ai-collaborative-development-preflight-AI协作开发前期规范/SKILL.md` | ⭐ AI 运行时执行规则 |
| `agents/openai.yaml` | Agent 元数据 |

完整参考文档和模板见 GitHub 仓库完整版。

## 版本

| 版本 | 核心变化 |
|------|----------|
| **v3.1.0** | 11阶段循环门控；强制覆盖清单；选项优劣+术语解释；完整性门控；防偏移回滚；LIGHT↔FULL升级路径 |
| v3.0.0 | 执行引擎重写；FULL/LIGHT双模式；状态机；硬约束 |
| v2.x | 完整双语项目脚手架；15步工作流 |

详见 [CHANGELOG.md](./CHANGELOG.md)

## 许可证

MIT License — [hanqingyan3293](https://github.com/hanqingyan3293)