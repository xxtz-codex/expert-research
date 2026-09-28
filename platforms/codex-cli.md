# Codex CLI (OpenAI) 安装指南

Codex CLI 支持 Agent Skills 开放标准，技能放在 `~/.codex/skills/`。

## 安装

```bash
mkdir -p ~/.codex/skills
cd ~/.codex/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

或手动把 `expert-research/` 文件夹复制到 `~/.codex/skills/`。

## Windows 路径

```
C:\Users\<你的用户名>\.codex\skills\expert-research\
```

## 验证

重启 codex，输入如"帮我调研 Obsidian 的免费替代品"，应命中技能按专家模板执行。

## 备注

- 技能名 kebab-case：`expert-research` ✓
- 默认用 `SKILL.md`（中文）；英文版把 `SKILL.en.md` 重命名为 `SKILL.md`
