# Kilo Code 安装指南

Kilo Code（VS Code 插件）原生支持 Agent Skills 标准。技能目录：

- 全局：`~/.kilo/skills/`（Windows：`C:\Users\<你的用户名>\.kilo\skills\`）
- 项目级：`.kilo/skills/`

## 安装（macOS / Linux）

```bash
# 全局
mkdir -p ~/.kilo/skills
cd ~/.kilo/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research

# 或项目级
mkdir -p <你的项目>/.kilo/skills
cd <你的项目>/.kilo/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

## 安装（Windows）

```powershell
# 全局
New-Item -ItemType Directory -Path "$HOME\.kilo\skills" -Force
cd "$HOME\.kilo\skills"
git clone https://github.com/xxtz-codex/expert-research.git expert-research

# 或项目级
New-Item -ItemType Directory -Path "<你的项目>\.kilo\skills" -Force
cd "<你的项目>\.kilo\skills"
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

## 正文超长：建议用 variants/split

Kilo 官方建议正文精简。本仓库完整版 `SKILL.md` 为 48.9KB，建议直接把 [`variants/split/`](../variants/split/) 整个目录复制为 `.kilo/skills/expert-research/`（精简路由 + references/ 全量模板按需加载）。

## 验证

在 Kilo Code 聊天框输入 `/reload` 重载，再打开 `/` 命令菜单，在 **Skills** 分组中应能看到 `expert-research`。问一个调研类问题，按专家模板执行即成功。

## 中英文版切换

- 默认使用 `SKILL.md`（中文版）
- 想用英文版：把目录里的 `SKILL.en.md` 重命名为 `SKILL.md`（先备份原文件）

## 官方文档来源

- https://kilo.ai/docs/customize/skills ✅ 已核实原文
