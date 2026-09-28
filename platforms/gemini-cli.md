# Gemini CLI 安装指南

Gemini CLI（Google 官方命令行工具）原生支持 Agent Skills 标准，且能直接从 Git 仓库安装。技能目录：

- 全局：`~/.gemini/skills/` 或 `~/.agents/skills/`
- 项目级：`.gemini/skills/`

## 方式 A：一键安装（推荐）

```bash
gemini skills install https://github.com/xxtz-codex/expert-research --consent
```

`--consent` 表示同意该技能的使用条款；不加则会交互询问。

## 方式 B：本地 link / 手动克隆

```bash
# 先克隆到任意位置
git clone https://github.com/xxtz-codex/expert-research.git ~/expert-research

# 再 link 进 skills 目录
gemini skills link ~/expert-research

# 或手动克隆到全局目录
mkdir -p ~/.gemini/skills
git clone https://github.com/xxtz-codex/expert-research.git ~/.gemini/skills/expert-research
```

## Windows 路径

```
C:\Users\<你的用户名>\.gemini\skills\expert-research\
C:\Users\<你的用户名>\.agents\skills\expert-research\
```

Gemini CLI 原生支持 `SKILL.md` + `references/` 布局，全量模板库按需加载，无需额外转换。

## 验证

```bash
gemini skills list
```

列表中应出现 `expert-research`。进入 `gemini` 交互会话，提一个调研类问题（如"帮我做 10 万块 3 年期理财框架"），命中技能按专家模板执行即成功。

## 中英文版切换

- 默认使用 `SKILL.md`（中文版）
- 想用英文版：把目录里的 `SKILL.en.md` 重命名为 `SKILL.md`（先备份原文件）

## 官方文档来源

- https://geminicli.com/docs/cli/skills ✅ 已核实原文
