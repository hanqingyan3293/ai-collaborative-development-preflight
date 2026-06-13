# MomoCrypt 开发规格

## 项目概述

MomoCrypt 是一个本地文件加密和伪装输出工具。它使用标准认证加密保护真实数据，再使用自定义密码本和多格式伪装输出形成项目特色。

## 核心流程

```text
原文件
↓
压缩
↓
标准认证加密
↓
自定义密码本扰乱
↓
伪装输出
```

## 技术栈

- Rust
- Tauri
- Vue
- TypeScript
- WASM 插件沙箱

## 伪装格式

- PNG
- JPG
- WAV
- DOCX
- TXT
- LOG
- CSS 颜色表

## 模块

| 模块 | 职责 |
|---|---|
| CryptoCore | 标准加密 |
| MomoCipher | 自定义密码本扰乱 |
| CarrierFormats | 伪装格式 |
| PluginRuntime | 插件沙箱 |
| UI | 用户界面 |
| History | 历史记录 |

## 验收标准

- 加密后解密 hash 一致。
- 错误密码无法解密。
- 伪装文件可被常规软件打开。
- 插件不能访问主密钥。
- 日志不包含敏感信息。
