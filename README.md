# AI协作开发前期规范 v2.2

让AI在写代码前先完成：理解 → 反问 → 决策 → 验证 → 规格输出

## 核心升级
- 选项式反问系统
- 每轮总结确认机制
- 防偏移机制
- 动态提问模块化
- Codex执行规范

## 这是什么

这是一个 **Codex Skill Plugin**，也是一个通用的 AI 协作开发前期规范。它确保 AI 在进入正式编码前：

1. 先复述理解你的项目构想
2. 分轮反问关键问题（方向级 → 功能级 → 工程级）
3. 锁定决策，防止后续随意改变
4. 检查风险和遗漏
5. 设计架构、数据、UI、安全
6. 定义验收标准
7. 输出可执行的开发规格

## 快速开始

```text
请按《AI协作开发前期规范》执行。先复述我的项目构想，再分轮反问关键问题；
在需求、技术栈、架构和验收标准未锁定前，不要直接进入正式实现。
```

详见 [QUICK_START.md](QUICK_START.md) 和 [docs/how-to-use-with-codex.md](docs/how-to-use-with-codex.md)

## 项目结构

```
├── SKILL.md              # Codex Skill 入口文件
├── .codex-plugin/        # Codex Plugin 配置
│   └── plugin.json
├── agents/               # UI 元数据
│   └── openai.yaml
├── docs/                 # 详细文档
├── templates/            # 开发模板（核心 + 高级）
├── checklists/           # 检查清单
├── examples/             # 示例项目
└── .github/              # Issue/PR 模板
```

## 许可证

MIT License - 详见 [LICENSE](LICENSE)
