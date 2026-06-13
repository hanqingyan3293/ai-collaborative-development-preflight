# 给 Codex 的操作教程：完善并同步 GitHub 仓库

## 目标

请把压缩包中的完整项目文件同步到这个 GitHub 仓库：

```text
hanqingyan3293/ai-collaborative-development-preflight
```

仓库地址：

```text
https://github.com/hanqingyan3293/ai-collaborative-development-preflight
```

## 背景

这是一个文档型 Skill 项目，名称为：

```text
AI协作开发前期规范 / AI Collaborative Development Preflight
```

用途是让 AI 在正式开发前先完成需求澄清、反问确认、决策锁定、架构规划、风险检查和验收设计。

用户已经把基础版本上传到 GitHub。现在需要用本压缩包中的版本覆盖和完善仓库，让它成为一个更完整、更合格的 GitHub Skill 项目。

## 你要做什么

1. 解压用户提供的 zip。
2. 将解压后的所有文件复制到仓库根目录。
3. 如果仓库已有同名文件，使用压缩包中的版本覆盖。
4. 保持目录结构。
5. 不要把文件放进额外嵌套目录。
6. 提交到 `main` 分支。

## 重要要求

根目录应该直接包含：

```text
README.md
README.en.md
QUICK_START.md
QUICK_START.en.md
skill.md
LICENSE
CONTRIBUTING.md
CONTRIBUTING.en.md
CODE_OF_CONDUCT.md
CHANGELOG.md
PROJECT_COMPLETION_REPORT.md
CODEX_UPLOAD_GUIDE.md
docs/
templates/
checklists/
examples/
.github/
```

不要变成：

```text
repo/ai-collaborative-development-preflight-v2/README.md
```

而应该是：

```text
repo/README.md
```

## 推荐 Git 命令

```bash
git clone https://github.com/hanqingyan3293/ai-collaborative-development-preflight.git
cd ai-collaborative-development-preflight

# 将 zip 解压后的根目录文件复制到当前目录，覆盖已有文件

git status
git add .
git commit -m "Improve AI Collaborative Development Preflight project"
git push origin main
```

如果仓库已有更新：

```bash
git pull origin main
```

如果出现冲突，以压缩包中的版本为准。

## 验收标准

完成后请检查：

1. README.md 是完整中文介绍。
2. README.en.md 是完整英文介绍。
3. skill.md 是双语 Skill，并包含核心流程、原则、输出格式和跳过规则。
4. docs/how-to-use-with-codex.md 存在。
5. templates/core/development-spec.md 存在。
6. checklists/preflight-checklist.md 存在。
7. examples/advanced/momo-crypt/development-spec.md 存在。
8. .github/ISSUE_TEMPLATE/ 存在多个 Issue 模板。
9. LICENSE 存在且为 MIT。
10. PROJECT_COMPLETION_REPORT.md 存在。

## 完成后告诉用户

请输出：

```text
已完成 GitHub 同步。
仓库：
commit hash：
主要新增/更新内容：
是否有冲突：
```
