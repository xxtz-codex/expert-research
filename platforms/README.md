# Platform Adaptation（平台适配）

> This skill (Agent Skills open standard) can be installed into all mainstream AI tools. Each file below is a step-by-step install guide for one platform. / 本技能符合 Agent Skills 开放标准，可装入市面主流 AI 工具。下方每个文件是单个平台的安装指南。

| Platform 平台 | File 文件 | Install Type 安装方式 |
|---|---|---|
| Claude Code | [claude-code.md](claude-code.md) | Skills folder 技能文件夹 |
| Doubao 豆包 | [doubao.md](doubao.md) | .user_skills folder or paste compact instructions |
| DeepSeek Harness (DSH) | [dsh.md](dsh.md) | ~/.agents/skills |
| Codex CLI (OpenAI) | [codex-cli.md](codex-cli.md) | ~/.codex/skills |
| Cursor | [cursor.md](cursor.md) | .cursor/skills |
| GitHub Copilot | [copilot.md](copilot.md) | .github/skills / .claude/skills / ~/.copilot/skills |
| Windsurf | [windsurf.md](windsurf.md) | .windsurf/skills / ~/.codeium/windsurf/skills |
| Zed | [zed.md](zed.md) | ~/.agents/skills / <worktree>/.agents/skills |
| Kilo Code | [kilo.md](kilo.md) | ~/.kilo/skills / .kilo/skills |
| Cline | [cline.md](cline.md) | .cline/skills（必须用 variants/split 拆分版） |
| Continue.dev | [continue.md](continue.md) | .continue/rules/<name>.md（需转换） |
| Gemini CLI | [gemini-cli.md](gemini-cli.md) | ~/.gemini/skills / ~/.agents/skills |
| ChatGPT (Custom GPT) | [chatgpt.md](chatgpt.md) | Paste compact instructions 粘贴浓缩指令 |
| Claude.ai | [claude-ai.md](claude-ai.md) | Project instructions 粘贴浓缩指令 |
| Other apps 其他助手 (Kimi/通义/智谱/讯飞…) | [other-apps.md](other-apps.md) | System prompt / role setting 系统提示/角色设定 |

**Compact instruction files 浓缩指令版（粘贴型平台用）:** [compact-zh.txt](../instructions/compact-zh.txt) · [compact-en.txt](../instructions/compact-en.txt)

## File structure 仓库文件结构

```
expert-research/
├── SKILL.md        ← 中文完整版技能主文件 (Chinese full version, 48.9KB)
├── SKILL.en.md     ← 英文完整版技能主文件 (English full version)
├── README.md       ← 中英双语介绍 (Bilingual README)
├── LICENSE         ← MIT
├── instructions/   ← 浓缩指令版 (Compact instruction text，粘贴型平台用)
│   ├── compact-zh.txt
│   └── compact-en.txt
├── platforms/      ← 各平台安装指南 (Per-platform install guides)
├── references/     ← 全量模板库引用文件 (Full template library, loaded on demand)
│   ├── prompt-template.md      (中文全量模板)
│   └── prompt-template.en.md   (English full templates, line-by-line translated)
├── variants/split/ ← 精简路由拆分变体 (Lightweight router split variant，限长平台用)
│   ├── SKILL.md / SKILL.en.md  (路由主文件，<5k tokens)
│   └── references/             (引用同一份全量模板库)
└── examples/       ← 使用示例
```

> Most folder-based tools only read `SKILL.md` — rename `SKILL.en.md` to `SKILL.md` when you want the English version to be the active one. / 大多数文件夹型工具只读 `SKILL.md`——想用英文版时把 `SKILL.en.md` 重命名为 `SKILL.md` 即可。

> **`references/`** holds the on-demand full template library (not auto-loaded; the main SKILL.md pulls it in only when a deep dive is needed). **`variants/split/`** is a slimmed router variant for platforms that enforce a short `SKILL.md` (e.g. Cline <5k tokens, Zed/Kilo/Doubao recommended <500 lines) — copy that whole directory in as the skill folder. / `references/` 是按需加载的全量模板库（不自动注入上下文）；`variants/split/` 是给限长平台用的精简路由变体——把整个目录当作技能文件夹复制进去即可。

## 核实状态说明 / Verification status

每个平台指南末尾都标注了官方文档来源，状态含义如下：

- ✅ = 已读官方原文（official docs page actually read）
- ⚠️ = 仅摘要或推断（summary / inference only，未逐字核对官方页面）
- ❌ = 未查到官方技能通道（no official SKILL.md channel found）
