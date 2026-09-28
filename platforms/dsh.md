# DeepSeek Harness (DSH) 安装指南

DSH 的 `@deepseek-ai/dsh-skill-filesystem` 提供者会从 `agentsHome`（默认 `~/.agents`）发现标准技能文件夹（Agent Skills 布局），无需打包成 npm 插件。

## 安装（Windows）

1. 打开 PowerShell，执行：

```powershell
New-Item -ItemType Directory -Path "$HOME\.agents\skills" -Force
Copy-Item "expert-research" "$HOME\.agents\skills\expert-research" -Recurse
```

或直接克隆：

```powershell
cd $HOME\.agents\skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

2. 重启 DSH Desktop（或在设置中重载 profile）

## 安装（macOS / Linux）

```bash
mkdir -p ~/.agents/skills
cd ~/.agents/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

## 原理说明（为什么能装）

- DSH 内核（0.1.5-rc.x）内置技能注册表 `@deepseek-ai/dsh-skill`，技能来源由 `dsh-skill-filesystem` 提供
- 该提供者发现目录：`DSH_AGENTS_HOME`（环境变量）→ `~/.agents`（默认），支持"目录包 + 扁平 Markdown"两种技能形态
- 技能名必须为 kebab-case（`expert-research` 符合）；`SKILL.md` 为技能主文件
- 你的 profile 里已有的 `dsh-our-free-model` 走的是 npm bundle 通道（`package.json → dsh.profile.bundles`），技能与插件是两套加载路径，互不冲突

## 验证

DSH 会话中输入调研类问题，模型应能命中 `expert-research` 技能并按模板执行；也可在 DSH 设置/插件面板查看已发现技能列表。

## 中英文版切换

- 默认加载 `SKILL.md`（中文版）
- 想用英文版：重命名 `SKILL.en.md` → `SKILL.md`

## 官方文档来源（核实状态）

- https://github.com/deepseek-ai/deepseek-harness/blob/main/docs/subsystems/skills.md ✅ 已核实原文
- https://www.npmjs.com/package/@deepseek-ai/dsh-skill-filesystem ✅ 已核实原文
- https://github.com/deepseek-ai/deepseek-harness/blob/main/docs/architecture.md ✅ 已核实原文
- 另注：无需 npm 插件打包；技能（`~/.agents/skills/` 目录包）与 Cordis 插件（bundle）是两条互不冲突的加载路径。
