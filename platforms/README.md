# Platform Adaptation（平台适配）

> This skill (Agent Skills open standard) can be installed into all mainstream AI tools. Each file below is a step-by-step install guide for one platform. / 本技能符合 Agent Skills 开放标准，可装入市面主流 AI 工具。下方每个文件是单个平台的安装指南。

| Platform 平台 | File 文件 | Install Type 安装方式 |
|---|---|---|
| Claude Code | [claude-code.md](claude-code.md) | Skills folder 技能文件夹 |
| Doubao 豆包 | [doubao.md](doubao.md) | .user_skills folder or paste compact instructions |
| DeepSeek Harness (DSH) | [dsh.md](dsh.md) | ~/.agents/skills |
| Codex CLI (OpenAI) | [codex-cli.md](codex-cli.md) | ~/.codex/skills |
| Cursor | [cursor.md](cursor.md) | .cursor/skills |
| ChatGPT (Custom GPT) | [chatgpt.md](chatgpt.md) | Paste compact instructions 粘贴浓缩指令 |
| Claude.ai | [claude-ai.md](claude-ai.md) | Project instructions 粘贴浓缩指令 |
| Other apps 其他助手 (Kimi/通义/智谱/讯飞…) | [other-apps.md](other-apps.md) | System prompt / role setting 系统提示/角色设定 |

**Compact instruction files 浓缩指令版（粘贴型平台用）:** [compact-zh.txt](../instructions/compact-zh.txt) · [compact-en.txt](../instructions/compact-en.txt)

## File structure 仓库文件结构

```
expert-research/
├── SKILL.md        ← 中文完整版技能主文件 (Chinese full version)
├── SKILL.en.md     ← 英文完整版技能主文件 (English full version)
├── README.md       ← 中英双语介绍 (Bilingual README)
├── LICENSE         ← MIT
├── instructions/   ← 浓缩指令版 (Compact instruction text)
│   ├── compact-zh.txt
│   └── compact-en.txt
├── platforms/      ← 各平台安装指南 (Per-platform install guides)
└── examples/       ← 使用示例
```

> Most folder-based tools only read `SKILL.md` — rename `SKILL.en.md` to `SKILL.md` when you want the English version to be the active one. / 大多数文件夹型工具只读 `SKILL.md`——想用英文版时把 `SKILL.en.md` 重命名为 `SKILL.md` 即可。
