# Cline 安装指南

Cline（VS Code 插件）原生支持 Agent Skills，但 **Experimental 功能默认关闭**，需手动打开；且官方强制要求 `SKILL.md` 正文 < 5k tokens——本仓库完整版 48.9KB 远超限制，**必须使用 `variants/split/` 精简拆分版**。

## 第 0 步：打开 Experimental 开关

VS Code → Cline 设置（齿轮图标）→ **Features** → 打开 **Enable Skills (Experimental)**。

## 第 1 步：用 variants/split 作为技能文件夹（必须）

不要直接用仓库根目录！把仓库的 [`variants/split/`](../variants/split/) **整个目录内容**复制为技能文件夹：

```
.cline/skills/expert-research/
├── SKILL.md            ← 精简路由（中文）
├── SKILL.en.md         ← 精简路由（英文）
└── references/
    ├── prompt-template.md
    └── prompt-template.en.md
```

### macOS / Linux

```bash
# 项目级（推荐，配合 docs/ 目录）
mkdir -p <你的项目>/.cline/skills
cp -r <本仓库克隆路径>/variants/split <你的项目>/.cline/skills/expert-research

# 或全局
mkdir -p ~/.cline/skills
cp -r <本仓库克隆路径>/variants/split ~/.cline/skills/expert-research
```

### Windows

```powershell
# 项目级
New-Item -ItemType Directory -Path "<你的项目>\.cline\skills" -Force
Copy-Item -Recurse "<本仓库克隆路径>\variants\split" "<你的项目>\.cline\skills\expert-research"

# 或全局
New-Item -ItemType Directory -Path "$HOME\.cline\skills" -Force
Copy-Item -Recurse "<本仓库克隆路径>\variants\split" "$HOME\.cline\skills\expert-research"
```

## 可识别的技能目录

Cline 按以下位置发现技能（任选其一放 `expert-research/`）：

- `.cline/skills/`（**推荐**，可带 `docs/` 子目录）
- `.clinerules/skills/`
- `.claude/skills/`（可保留 `references/` 原名，Cline 兼容读取）
- 全局：`~/.cline/skills/`

## 验证

重启 VS Code / Cline，打开 Cline 面板切到 **Skills** 标签页，列表中应出现 `expert-research`；对话中 Cline 会通过 `use_skill` 工具调用它。提一个调研类问题，按精简路由命中对应专家模板即成功。

## 中英文版切换

- `variants/split/` 内同时带 `SKILL.md`（中文路由）与 `SKILL.en.md`（英文路由）
- 想用英文版：把 `SKILL.en.md` 重命名为 `SKILL.md`（先备份原文件）

## 官方文档来源

- https://docs.cline.bot/customization/skills ✅ 已核实原文
