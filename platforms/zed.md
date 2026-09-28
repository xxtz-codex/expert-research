# Zed 安装指南

Zed 原生支持 Agent Skills 标准。技能目录（**注意纠正**：不是 `~/.config/zed/skills`，也不是 `.zed/skills/`）：

- 全局：`~/.agents/skills/`
- 项目（worktree）：`<worktree>/.agents/skills/`

## 安装（macOS / Linux）

```bash
# 全局
mkdir -p ~/.agents/skills
cd ~/.agents/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research

# 或项目级
mkdir -p <你的项目>/.agents/skills
cd <你的项目>/.agents/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

## 安装（Windows）

```powershell
# 全局
New-Item -ItemType Directory -Path "$HOME\.agents\skills" -Force
cd "$HOME\.agents\skills"
git clone https://github.com/xxtz-codex/expert-research.git expert-research

# 或项目级
New-Item -ItemType Directory -Path "<你的项目>\.agents\skills" -Force
cd "<你的项目>\.agents\skills"
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

## 正文超长：建议用 variants/split

Zed 官方建议单个 `SKILL.md` 正文不超过约 500 行。本仓库完整版 `SKILL.md` 为 48.9KB（约 1300+ 行），若你的 Zed 版本对长度敏感，直接把仓库的 [`variants/split/`](../variants/split/) 整个目录复制为 `.agents/skills/expert-research/`（精简路由 + 全量 references 仍在，按需加载）。

## 在 Zed 里创建技能

也可在 agent 面板输入 `/create-skill` 走官方向导，再把本仓库内容贴入生成的技能文件夹。

## 验证

打开 Zed agent 面板，按 `Ctrl+,`（macOS: `Cmd+,`）→ **AI** → **Skills**，列表中应能看到 `expert-research`。再问调研类问题，按专家模板执行即成功。

## 中英文版切换

- 默认使用 `SKILL.md`（中文版）
- 想用英文版：把目录里的 `SKILL.en.md` 重命名为 `SKILL.md`（先备份原文件）

## 官方文档来源

- https://zed.dev/docs/ai/skills ✅ 已核实原文
