# Claude Code 安装指南

Claude Code 原生支持 Agent Skills 标准，把技能文件夹放进 skills 目录即可。

## 方式 A：克隆安装（推荐）

```bash
mkdir -p ~/.claude/skills
cd ~/.claude/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

## 方式 B：手动复制

把本仓库的 `expert-research/` 文件夹整个复制到：

```
Windows:  C:\Users\<你的用户名>\.claude\skills\expert-research\
macOS:    ~/.claude/skills/expert-research/
```

也可以放进**某个项目**目录下：`<项目>/.claude/skills/expert-research/`（仅该项目可用）。

## 验证

重启 Claude Code，输入任意调研类问题（如"帮我找 Obsidian 的同类笔记软件"），若命中技能会按专家模板执行。

## 中英文版切换

- 默认使用 `SKILL.md`（中文版）
- 想用英文版：把目录里的 `SKILL.en.md` 重命名为 `SKILL.md`（先备份原文件）

## 深度版

任意模板末尾追加：`深度：深度版（追加通用盲点清单）` 即可启用 12 类盲点核查。

## 官方文档来源（核实状态）

- https://code.claude.com/docs/en/skills ✅ 已核实原文
- 另注：从 GitHub 下载 ZIP 解压后目录名是 `expert-research-main`，须改名为 `expert-research`；保留名 `synced/anthropic-skills` 不可用。
