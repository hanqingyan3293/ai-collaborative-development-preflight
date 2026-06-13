# AI协作开发前期规范

> 让 AI 先想清楚，再写代码。  
> Make AI clarify, plan, and lock decisions before implementation.

《AI协作开发前期规范》是一套面向所有 AI 协作开发场景的开源流程规范。它通过 `skill.md`、模板、检查表、示例和 Codex 使用说明，帮助用户在正式开发前完成需求澄清、反问确认、决策锁定、架构规划、风险检查和验收设计。

English: [README.en.md](./README.en.md)

## 项目定位

这是一个文档型、Skill 型、流程型开源项目，不是普通软件库。它的目标是让 ChatGPT、Codex、Cursor、Claude、Copilot 等 AI 工具在开发前先完成“项目预检”，避免需求不清、技术栈混乱、架构返工和验收标准缺失。

## 解决什么问题

很多 AI 协作开发失败，不是因为 AI 不会写代码，而是因为一开始就直接进入实现：

- 用户只说了一个想法，没有定义边界。
- AI 没有反问关键问题。
- 功能范围没有锁定。
- 技术栈随意变化。
- 架构、数据结构、接口、UI、安全、测试没有提前设计。
- 项目做到一半不断返工。
- 最后无法判断“是否完成”。

本项目把这套前置过程做成可复用的规范。

## 适用范围

适用于几乎所有 AI 协作项目：

- 桌面软件
- Web 网站
- 移动 App
- 浏览器插件
- 后端服务
- 命令行工具
- AI 工具
- 游戏
- 自动化脚本
- 数据处理工具
- 文档系统
- 知识库系统
- 插件系统
- 开源项目规划

## 快速开始

把下面这段话发给 AI：

```text
请按《AI协作开发前期规范》执行。先复述我的项目构想，再分轮反问关键问题；在需求、技术栈、架构和验收标准未锁定前，不要直接进入正式实现。每轮回答后请输出：已确定、未确定、存在风险、下一步问题。
```

更多说明见：[QUICK_START.md](./QUICK_START.md)

## 核心流程

```text
用户提出构想
↓
AI 复述理解
↓
AI 识别项目类型
↓
AI 分轮反问
↓
用户选择
↓
AI 记录决策
↓
AI 检查遗漏、矛盾和风险
↓
AI 设计功能、流程、架构、数据、UI、权限、测试和验收
↓
AI 生成开发规格文档
↓
再进入代码生成阶段
```

## 核心文件

| 文件 / 目录 | 用途 |
|---|---|
| `skill.md` | 给 AI 读取的双语执行规则 |
| `QUICK_START.md` | 快速复制使用的启动提示词 |
| `docs/` | 完整流程说明、问题库、Codex 使用说明 |
| `templates/` | 需求澄清、决策锁定、开发规格等模板 |
| `checklists/` | 前期检查、AI 编码检查、安全检查、发布检查 |
| `examples/` | 桌面、Web、AI 工具、游戏、浏览器插件、自动化脚本、高级 MomoCrypt 示例 |
| `.github/` | Issue 与 Pull Request 模板 |
| `CODEX_UPLOAD_GUIDE.md` | 给 Codex 上传/同步 GitHub 仓库的教程 |

## 推荐使用方式

### 方式一：聊天 AI

把 `QUICK_START.md` 的启动提示词复制给 AI，然后描述项目构想。

### 方式二：Codex / Cursor

把本仓库作为项目规则或上下文，让 AI 优先读取：

1. `skill.md`
2. `docs/workflow.md`
3. `templates/core/development-spec.md`
4. 对应项目类型的 `examples/`

### 方式三：开源项目模板

复制本仓库中的模板和检查表，放进自己的项目仓库，用于规范 AI 开发流程。

## 项目成熟度

当前版本已经包含完整项目结构、核心 Skill、模板、检查表、示例和 Codex 教程。它可以作为一个可公开发布的 Skill 项目继续迭代。

## 贡献

欢迎贡献：

- 新模板
- 新示例
- 更好的中英文翻译
- 更多项目类型问题库
- Codex / Cursor / Claude / ChatGPT 使用经验

请阅读 [CONTRIBUTING.md](./CONTRIBUTING.md)。

## 许可证

MIT License。见 [LICENSE](./LICENSE)。

## Language / 语言

- 中文：当前文件
- English: [README.en.md](./README.en.md)
