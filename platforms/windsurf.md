# Windsurf 安装指南

Windsurf（Codeium 出品的 AI IDE）原生支持 Agent Skills 标准。技能目录：

- 工作区（项目级）：`.windsurf/skills/`
- 全局：`~/.codeium/windsurf/skills/`

> 注意：全局目录在 `~/.codeium/windsurf/` 下，**不是** `~/.windsurf/`。

## 安装（macOS / Linux）

```bash
# 全局
mkdir -p ~/.codeium/windsurf/skills
cd ~/.codeium/windsurf/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research

# 或工作区级
mkdir -p <你的项目>/.windsurf/skills
cd <你的项目>/.windsurf/skills
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

## 安装（Windows）

```powershell
# 全局
New-Item -ItemType Directory -Path "$HOME\.codeium\windsurf\skills" -Force
cd "$HOME\.codeium\windsurf\skills"
git clone https://github.com/xxtz-codex/expert-research.git expert-research

# 或工作区级
New-Item -ItemType Directory -Path "<你的项目>\.windsurf\skills" -Force
cd "<你的项目>\.windsurf\skills"
git clone https://github.com/xxtz-codex/expert-research.git expert-research
```

## UI 方式安装

打开 Cascade 面板 → 右上角 **⋮** → **Skills** → **+ Workspace**（工作区技能）或 **+ Global**（全局技能），按提示选择技能文件夹。

## 验证

在 Cascade 对话中输入 `@expert-research` 唤起技能，再提一个调研类问题（如"帮我规划学习 Rust 的路线"），按专家五段式输出即成功。

## 中英文版切换

- 默认使用 `SKILL.md`（中文版）
- 想用英文版：把目录里的 `SKILL.en.md` 重命名为 `SKILL.md`（先备份原文件）

## 官方文档来源

- https://docs.windsurf.com/windsurf/cascade/skills ✅ 已核实原文
