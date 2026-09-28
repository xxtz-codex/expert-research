---
name: expert-research
description: "Expert-grade multi-type deep research and decision-support skill. 14 expert templates: tool/software alternative selection, learning path design, competitor analysis, local environment setup, content strategy, evidence-based medical consultation, resume/career optimization, purchase decision, travel planning, investment planning, home renovation material selection, life planning, relationship communication coaching, fitness training. Use when the user asks for similar solutions/alternatives ('find me X like Y'), deep research, expert-grade planning, analysis, or decision support - in Chinese or English. Each template includes expert workflow, hidden blind-spot dimensions, quality red lines, output format, and iteration follow-ups."
---
# Expert Research & Decision Support（专家级多类型调研与决策技能）

本技能内置 14 类专家模板 + 兜底路由。流程：输入解析 → 类型识别 → 按对应模板执行（专家流程 → 隐性维度 → 质量红线 → 输出格式 → 迭代追问）→ 通用盲点（可选深度版）→ 交付自检。

## 完整模板库（执行前先读）

`references/prompt-template.md` 是 v8 全量模板库：14 类模板正文 + 兜底模板 + 12 类通用盲点清单 + 交付自检清单 + 沉淀输出格式 + 使用说明。按用户问题类型选取对应模板执行。

## 类型路由

| 用户问题类型 | 模板 |
|---|---|
| 工具/软件替代品选型 | 模板 1 |
| 系统学习某技能/知识 | 模板 2 |
| 产品/竞品分析 | 模板 3 |
| 本地环境/配置方案 | 模板 4 |
| 内容创作选题 | 模板 5 |
| 健康/医学咨询 | 模板 6 |
| 简历/求职优化 | 模板 7 |
| 消费/购物决策 | 模板 8 |
| 旅行规划 | 模板 9 |
| 投资理财 | 模板 10 |
| 装修选材 | 模板 11 |
| 人生规划 | 模板 12 |
| 情侣/亲密关系沟通 | 模板 13 |
| 健身训练 | 模板 14 |
| 类型不确定 | 兜底模板 |

## 深度开关

用户说"深度/更全面"时，追加 `references/prompt-template.md` 中的 12 类通用盲点清单逐条核查。

## 合规红线

医学只做循证、不诊断不处方；理财只给框架、不构成投资建议、不荐个股；情侣沟通中立不评判、不给分手断言；健身给安全红线、不诊断伤病。

## 交付自检（每次交付前）

来源链接真实可打开；每条结论标注 ✅已核实 / ⚠️待验证 / ❌未查到；事实与推断分离；隐性维度逐条核查；对比表有比较轴；无编造；给出取舍与代价；医学/理财/情侣/健身合规提示齐备。

## 沉淀

用 `references/prompt-template.md` 末尾的【沉淀输出格式】把结论存入用户知识库（Obsidian 等）。
