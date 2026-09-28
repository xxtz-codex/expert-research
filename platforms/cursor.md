# Cursor 安装指南

Cursor（基于 VS Code 的 AI IDE）支持 `.cursor/skills/` 目录加载技能（Agent Skills 标准，2025 后版本）。

## 安装

```bash
# 全局（当前用户所有项目可用）
mkdir -p ~/.cursor/skills
cd ~/.cursor/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research

# 或项目级（仅当前项目）
mkdir -p <你的项目>/.cursor/skills
cd <你的项目>/.cursor/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

## Windows 路径

```
C:\Users\<你的用户名>\.cursor\skills\expert-research\
```

## 验证

重启 Cursor，在对话中问调研类问题，命中技能即按专家模板执行。

## 备注

- 如果 Cursor 版本较旧不支持 skills 目录，改用 Custom Instructions：设置 → 把 [`instructions/compact-zh.txt`](../instructions/compact-zh.txt) 粘贴到 Rules / 自定义指令
- 默认用 `SKILL.md`（中文）；英文版重命名 `SKILL.en.md` → `SKILL.md`

## 官方文档来源（核实状态）

- https://cursor.com/docs/skills ✅ 已核实原文
- 另注：`name` = 文件夹名，须小写 kebab-case；Cursor 兼容识别 `.agents/`、`.claude/`、`.codex/` 下的 skills 目录；Cloud Agents 只同步 `~/.cursor/skills/`。
