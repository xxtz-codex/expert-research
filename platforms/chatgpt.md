# ChatGPT（Custom GPT / 项目说明）安装指南

ChatGPT 不支持技能文件夹，通过 **Custom GPT 系统提示** 或 **项目说明（Instructions）** 粘贴浓缩指令版即可获得完整能力。

## 方式 A：创建 Custom GPT

1. 打开 https://chatgpt.com/gpts/editor 或 ChatGPT → Explore GPTs → **Create**
2. Name 填：`Expert Research（专家调研助手）`
3. 在 **Instructions** 框粘贴 [`instructions/compact-zh.txt`](../instructions/compact-zh.txt) 全文（或英文版 `compact-en.txt`）
4. （可选）Description 填：`14 类专家模板的深度调研与决策助手`
5. Save → 之后任何会话都能调用

## 方式 B：项目 Instructions（不需要建 GPT）

1. 打开任意 ChatGPT 项目 → Project 设置 → **Instructions**
2. 粘贴 `compact-zh.txt` 全文 → 保存

## 验证

在新会话输入：`用模板 1 帮我找本地免费的笔记软件`，按专家五段式输出即成功。

## 备注

- 浓缩版覆盖：14 类模板路由 + 五段结构（专家流程/隐性维度/质量红线/输出格式/迭代追问）+ 深度版开关 + 交付自检
- 英文场景粘贴 `compact-en.txt`

## 官方文档来源（核实状态）

- https://help.openai.com/en/articles/20001066-skills-in-chatgpt ✅ 已核实原文
- 另注：ChatGPT 官方 Skills 上传（Plugins→Skills）仅 Business / Enterprise / Edu 可用；免费与 Plus 账号走 Custom GPT 粘贴浓缩指令（即本文方式 A/B）。
