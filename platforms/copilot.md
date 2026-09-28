# GitHub Copilot 安装指南

GitHub Copilot（VS Code / Visual Studio 中的 agent 模式）原生支持 Agent Skills 标准。它会按顺序扫描以下技能目录：

- 项目级：`.github/skills/`、`.claude/skills/`
- 全局：`~/.copilot/skills/`

## 方式 A：克隆安装（推荐）

```bash
# 全局（所有项目可用）
mkdir -p ~/.copilot/skills
cd ~/.copilot/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research

# 或项目级（仅当前仓库）
mkdir -p <你的项目>/.github/skills
cd <你的项目>/.github/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

## 方式 B：手动复制

把本仓库 `expert-research/` 文件夹整个复制到下列任一位置：

```
全局 Windows:  C:\Users\<你的用户名>\.copilot\skills\expert-research\
全局 macOS/Linux: ~/.copilot/skills/expert-research/
项目级:        <项目>\.github\skills\expert-research\
```

## 方式 C：gh CLI（public preview）

```bash
gh skill install https://github.com/xxtz-codex/expert-research
```

> 该命令目前为 public preview，语法与可用范围以 `gh skill --help` 为准；不稳定时用方式 A/B。

## 验证

重启 VS Code，打开 Copilot Chat 切到 agent 模式，在聊天框输入：

```
/skills
```

列表中应出现 `expert-research`；再问一个调研类问题（如"帮我找 Obsidian 的免费替代品"），命中技能即按专家模板执行。

## 中英文版切换

- 默认使用 `SKILL.md`（中文版）
- 想用英文版：把目录里的 `SKILL.en.md` 重命名为 `SKILL.md`（先备份原文件）

## 官方文档来源

- https://docs.github.com/en/copilot/concepts/agents/about-agent-skills ✅ 已核实原文
