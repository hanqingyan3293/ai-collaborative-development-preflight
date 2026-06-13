# AI协作开发前期规范

> 让 AI 先想清楚，再写代码。  
> Make AI clarify, plan, and lock decisions before writing code.

《AI协作开发前期规范》是一套面向所有 AI 协作开发场景的开源流程规范。它要求 AI 在正式进入实现阶段前，先完成需求理解、反问澄清、决策锁定、遗漏检查、架构规划、测试验收设计和开发规格输出。

English: [README.en.md](./README.en.md)

## 为什么需要这个项目

很多 AI 编程失败，不是因为 AI 不会写代码，而是因为开始写代码前没有把需求、边界、技术栈、架构和验收标准说清楚。

常见问题包括：

- 用户只描述了想法，没有明确功能边界。
- AI 没有反问，直接开始写代码。
- 技术栈随意变化。
- 数据结构和文件格式没有提前定义。
- UI 交互、异常处理、安全边界被忽略。
- 后续开发时不断返工。
- 验收标准不清楚，无法判断“是否完成”。

这个项目把“AI 开发前置工作”规范成可复用的流程、Skill、模板、检查表和示例。

## 适用范围

适用于所有使用 AI 协作开发的项目，包括但不限于：

- 桌面软件
- Web 网站
- 移动 App
- 浏览器插件
- AI 工具
- 游戏
- 自动化脚本
- 后端服务
- 数据处理工具
- 文档系统
- 知识库系统
- 插件系统
- 开源项目规划

## 快速开始

把下面这段发给 AI：

```text
请按《AI协作开发前期规范》执行。先复述我的项目构想，再分轮反问关键问题；在需求、技术栈、架构和验收标准未锁定前，不要直接写正式代码。每轮回答后请输出：已确定、未确定、存在风险、下一步问题。
```

更多说明见：[QUICK_START.md](./QUICK_START.md)

## 核心文件

- [skill.md](./skill.md)：给 AI 读取和执行的双语 Skill 规则。
- [docs/](./docs/)：完整流程说明和问题库。
- [templates/](./templates/)：开发前期模板。
- [checklists/](./checklists/)：检查清单。
- [examples/](./examples/)：不同类型项目的完整示例。
- [.github/](./.github/)：Issue 与 PR 模板。

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

## 目录结构

```text
.
├─ README.md
├─ README.en.md
├─ QUICK_START.md
├─ QUICK_START.en.md
├─ skill.md
├─ LICENSE
├─ CONTRIBUTING.md
├─ CONTRIBUTING.en.md
├─ CODE_OF_CONDUCT.md
├─ CHANGELOG.md
├─ docs/
├─ templates/
├─ checklists/
├─ examples/
└─ .github/
```

## 项目状态

当前版本为规范和模板项目，不包含 CLI、网站或应用程序。后续可以扩展为：

- CLI 工具
- Web 表单生成器
- VS Code / Cursor 模板
- GitHub Issue 工作流
- AI Agent 前置检查器

## 贡献

欢迎贡献模板、示例、翻译和改进建议。请阅读 [CONTRIBUTING.md](./CONTRIBUTING.md)。

## 许可证

MIT License。见 [LICENSE](./LICENSE)。

## Language / 语言

- 中文：当前文件
- English: [README.en.md](./README.en.md)
