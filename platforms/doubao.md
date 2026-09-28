# 豆包（Doubao）安装指南

豆包支持两种方式：技能文件夹（完整版）或自定义指令（浓缩版）。

## 方式 A：技能文件夹（完整版，推荐）

把 `expert-research` 文件夹放入豆包的技能库目录：

```
<豆包工作区>\workspace\.user_skills\expert-research\
```

（把仓库克隆或解压到该目录，确保 `SKILL.md` 在 `expert-research\` 下。）

## 方式 B：自定义指令（浓缩版，所有豆包版本通用）

1. 打开豆包 → 设置 → **自定义指令 / 角色设定 / 系统提示**
2. 把 [`instructions/compact-zh.txt`](../instructions/compact-zh.txt) 的全文粘贴进去
3. 保存后，任意新会话都会带上专家调研能力

## 验证

新建会话，输入：`用模板 1 帮我找免费的本地笔记软件`——若按专家五段式输出即安装成功。

## 提示

- 浓缩版覆盖 14 类模板路由 + 五段结构 + 深度版开关 + 交付自检，功能与完整版等价，适合字符受限的场景
- 豆包内也可把本技能放 `workspace/.user_skills/` 目录获得完整版能力

## 官方文档来源（核实状态）

- https://www.doubao.com/work/docs/zh-cn/articles/081010973544-skills ✅ 已核实原文
- https://www.volcengine.com/docs/86681/2137204 ✅ 已核实原文
- 另注：`name` 须为小写字母 / 数字 / 连字符，不能含中文；`description` 中文/英文均可；正文 >500 行官方建议拆分 → 用 [`variants/split/`](../variants/split/)。
