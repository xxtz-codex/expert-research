# Continue.dev 安装指南

Continue.dev（VS Code / JetBrains 插件）**没有 SKILL.md 概念**，不直接读取本仓库的技能文件夹。它的等价能力是 **Rules**（`.continue/rules/<name>.md`）与 **Prompts**。因此本技能需要**转换**：把 `SKILL.md` 的核心内容转成一条 rule / 一个 prompt，而不是整包拷贝。

## 第 1 步：创建 Rules 文件

在项目或全局 Continue 配置目录新建：

```
Windows:  C:\Users\<你的用户名>\.continue\rules\expert-research.md
macOS/Linux: ~/.continue/rules/expert-research.md
项目级:        <项目>\.continue\rules\expert-research.md
```

文件 frontmatter 至少要有 `name`，可选 `alwaysApply: false` 与 `invokable: true`：

```markdown
---
name: expert-research
description: 14 类专家模板的深度调研与决策助手（按需调用，不常驻）
alwaysApply: false
---
```

## 第 2 步：粘贴转换后的内容

frontmatter 下面，粘贴本仓库 [`instructions/compact-zh.txt`](../instructions/compact-zh.txt) 的全文（英文场景用 `compact-en.txt`），或粘贴精简路由 [`variants/split/SKILL.md`](../variants/split/SKILL.md) 的正文。

> ⚠️ **不要**把 48.9KB 的完整版 `SKILL.md` 设为 `alwaysApply: true` 常驻——会撑爆每次请求的上下文。保持 `alwaysApply: false` / `invokable: true`，让模型按需调用。

## 验证

打开 Continue 侧边栏，点工具栏**铅笔图标**（Rules 面板），应能看到 `expert-research` 这条 rule。在对话中 `/expert-research` 调用它，再提调研类问题，按专家五段式输出即成功。

## 与 Prompts 的关系

Continue 也支持自定义 slash prompt（`.continue/prompts/`）。若你更习惯 `/expert-research` 显式触发，可把同一段内容再存一份为 `.continue/prompts/expert-research.md`，效果等价。

## 中英文版切换

- 粘贴 `compact-zh.txt` = 中文版
- 粘贴 `compact-en.txt` = 英文版

## 官方文档来源

- https://docs.continue.dev/customize/rules ✅ 已核实原文
