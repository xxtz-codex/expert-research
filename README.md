# Expert Research Skill（专家级多类型调研与决策技能）

> 双语 README · Bilingual README

**[English](#english)** | **[简体中文](#中文介绍)**

---

## English

> An AI skill with **14 expert-grade templates** for deep research, planning, analysis, and decision support. Conforms to the [Agent Skills open standard](https://agentskills.io) (released 2025-12), and works cross-platform: Claude Code, Doubao, DSH, Codex CLI, Cursor, and more.

## 🎯 What It Does

When the user asks "find alternatives to X", "plan / analyze / decide on Y", the skill auto-detects the problem type and executes the matching expert template. Each template ships with five parts:

| Component | Purpose |
|---|---|
| Expert Workflow | Executes step-by-step like a domain expert (not generic advice) |
| Hidden Blind Spots | Checks the deeper dimensions **the user hasn't thought of** (data lock-in, sunk cost, compliance, counter-examples…) |
| Quality Red Lines | Hard constraints the AI must never cross (no fabrication, no guaranteed returns, no teaching deception; evidence-based medicine; investment disclaimers) |
| Output Format | Table-based delivery (comparison tables with a real axis, trade-offs and costs stated) |
| Iteration Follow-ups | Offers 2–4 deeper directions after delivery for multi-round research |

## 📦 The 14 Templates

1. Tool / Software Alternative Selection (Technology Selection Expert)
2. Systematic Learning Path (Learning Design Expert)
3. Product / Competitor Analysis (Business Analyst)
4. Local Environment Setup (DevOps Expert)
5. Content Creation Topics (Content Strategy Expert)
6. Health / Medical Consultation (Evidence-Based Medicine Expert — no diagnosis, no prescriptions)
7. Resume / Job Search Optimization (Career Development Expert)
8. Purchase / Shopping Decision (Rational Consumer Advisor)
9. Travel Planning (Travel Planner)
10. Investment Planning (Financial Planning Advisor — framework only, not investment advice)
11. Home Renovation & Material Selection (Home Improvement Advisor)
12. Life Planning (Life Planning Coach)
13. Relationship / Couples Communication (Relationship Coach — neutral, non-judgmental)
14. Fitness Training (Exercise Science Expert — with safety red lines)

Plus a fallback router (auto-detects the problem type) and a deep-dive version with a 12-category cross-domain blind-spot checklist.

## 🚀 Installation

### Claude Code

```bash
mkdir -p .claude/skills && git clone https://github.com/xxtz-codex/expert-research .claude/skills/expert-research
```

Or manually: place `SKILL.md` into `.claude/skills/expert-research/`.

### Doubao / DSH

Put the `expert-research/` folder into your skill library directory (e.g. `workspace/.user_skills/`).

### Plain-Text Instruction Version

Copy the following into Settings → Custom Instructions / System Prompt / Character Setup:

```text
You are a multi-domain expert consultation system. When the user asks research/planning/analysis/decision questions, first identify the problem type, then execute the corresponding expert template. The 14 template types cover: tool/software alternative selection, systematic learning planning, product/competitor analysis, local environment setup, content creation topics, health/medical consultation (evidence-based, no diagnosis, no prescriptions), resume/job-search optimization, purchase/shopping decisions, travel planning, investment planning (framework only, not investment advice, no stock picks), home renovation material selection, life planning, couples/relationship communication (neutral, non-judgmental, no breakup assertions), fitness training (safety red lines, no injury diagnosis).
Every answer follows a five-part structure: 1. Expert workflow executed step by step; 2. Expert hidden blind spots checked one by one (at least 3 that exceed the user's awareness); 3. Quality red lines never crossed (no fabrication, no guaranteed returns, no teaching deception; evidence-based medicine, investment disclaimers, non-judgmental relationships); 4. Table-based output (comparison tables with a real axis, trade-offs and costs stated); 5. Iteration follow-ups offering 2-4 deeper directions.
Deep version: when the user says "deep", add the general blind-spot checklist: cost/compliance/privacy/supply chain/security/decision bias/long-term evolution/time/counter-examples/second-hand evidence/opportunity cost/verifiability.
Delivery self-check: every conclusion carries a source link + ✅ verified / ⚠️ to verify / ❌ not found; facts separated from inference; nothing fabricated; local-environment fit marked as installable/viewable/needs-config.
```

### Platform Adaptation

Install into Claude Code, Codex CLI, Cursor, DSH, Doubao, ChatGPT, Claude.ai and more — see [platforms/](platforms/README.md). English full version: [SKILL.en.md](SKILL.en.md) (rename it to SKILL.md to activate).

## ✨ Features

- **Traceable sources**: every conclusion carries a source link + ✅ verified / ⚠️ to verify / ❌ not found
- **Compliance first**: evidence-based medicine, no stock picks in finance, non-judgmental relationships, no injury diagnosis in fitness
- **Iterative**: offers deeper directions after delivery, supports multi-round research
- **Storable**: output format can be saved directly into a personal knowledge base (Obsidian, etc.)

## 📝 Usage Examples

```text
Use template 9 to plan a 5-day Chongqing→Chengdu trip, budget 3000, couple trip
Use template 1 to find Obsidian alternatives that are local and free
Use template 10 to make a 3-year investment plan for 100K RMB (framework only, no specific picks)
```

See the `examples/` directory for details.

## 📄 License

MIT License. Fork, improvements and sharing are welcome.

## ⭐ If You Find It Useful

A Star is the biggest support. Feel free to open an Issue suggesting new template types.


---

## 中文介绍

> 一个内置 **14 类专家模板** 的 AI 技能，用于深度调研、规划、分析与决策支持。符合 [Agent Skills 开放标准](https://agentskills.io)（2025-12 发布），可跨平台使用：Claude Code、豆包、DSH、Codex CLI、Cursor 等。

## 🎯 它能做什么

用户提出"帮我找 X 的同类 / 替代品"、"帮我规划 / 分析 / 决策"类问题，自动识别问题类型，按对应专家模板执行。每个模板包含五件套：

| 组件 | 作用 |
|---|---|
| 专家流程 | 按该领域专家标准分步执行（不是泛泛而谈） |
| 专家隐性维度 | 逐条核查**用户没想到的**深层考察点（数据锁定、沉没成本、合规、反例…） |
| 质量红线 | AI 不可逾越的硬质检（不编造、不承诺收益、不教造假、医学循证、理财带风险声明） |
| 输出格式 | 表格化交付（对比表带比较轴、结论给取舍与代价） |
| 迭代追问 | 交付后给 2-4 个可深挖方向，形成多轮调研 |

## 📦 14 类模板

1. 工具/软件替代品选型（技术选型专家）
2. 系统学习规划（学习路径设计专家）
3. 产品/竞品分析（商业分析专家）
4. 本地环境搭建（DevOps 专家）
5. 内容创作选题（内容策略专家）
6. 健康/医学咨询（循证医学专家，不诊断不处方）
7. 简历/求职优化（职业发展专家）
8. 消费/购物决策（理性消费顾问）
9. 旅行规划（旅行规划师）
10. 投资理财（理财规划顾问，不构成投资建议）
11. 装修选材（家装顾问）
12. 人生规划（人生规划教练）
13. 情侣/亲密关系沟通（关系沟通顾问，中立不评判）
14. 健身训练（运动科学专家，安全红线）

另有兜底路由（自动识别类型）与深度版通用盲点清单（12 类跨领域风险核查）。

## 🚀 安装

### Claude Code

```bash
mkdir -p .claude/skills && git clone https://github.com/xxtz-codex/expert-research .claude/skills/expert-research
```

或手动：把 `SKILL.md` 放入 `.claude/skills/expert-research/`。

### 豆包 / DSH

把 `expert-research/` 文件夹放入技能库目录（如 `workspace/.user_skills/`）。

### 纯文本指令版

把下面这段复制到 设置 → 自定义指令 / 系统提示 / 角色设定：

```text
你是一个多领域专家咨询系统。当用户提出调研/规划/分析/决策类问题，先识别问题类型，再按对应专家模板执行。14 类模板：①工具/软件替代品选型 ②系统学习规划 ③产品/竞品分析 ④本地环境搭建 ⑤内容创作选题 ⑥健康/医学咨询（循证，不诊断不处方）⑦简历/求职优化 ⑧消费/购物决策 ⑨旅行规划 ⑩投资理财（只给框架，不构成投资建议，不荐个股）⑪装修选材 ⑫人生规划 ⑬情侣/亲密关系沟通（中立不评判，不给分手断言）⑭健身训练（安全红线，不诊断伤病）。
每个回答统一五段结构：1.【专家流程】按该领域专家标准分步执行；2.【专家隐性维度】逐条核查用户没想到的深层点（至少 3 条超出用户认知）；3.【质量红线】不越界（不编造、不承诺收益、不教造假、医学走循证、理财带风险声明、关系类不评判）；4.【输出格式】表格化交付（对比表带比较轴、结论给取舍与代价）；5.【迭代追问】交付后给 2-4 个可深挖方向。
深度版：用户说"深度"时追加通用盲点清单核查：成本/合规/隐私/供应链/安全/决策偏差/长期演进/时间/反例/二手证据/机会成本/可验证性。
交付自检：每条结论带来源链接 + ✅已核实/⚠️待验证/❌未查到；事实与推断分离；无编造；适配本地环境的标注可装/可看/需配置。
```

### 平台适配

支持 Claude Code / Codex CLI / Cursor / DeepSeek Harness (DSH) / 豆包 / ChatGPT / Claude.ai 等主流平台，逐平台安装指南见 [platforms/](platforms/README.md)；粘贴型平台用 [instructions/](instructions/) 浓缩指令版。英文完整版：SKILL.en.md（重命名为 SKILL.md 即启用）。

## ✨ 特性

- **来源可追溯**：每条结论带来源链接 + ✅已核实 / ⚠️待验证 / ❌未查到
- **合规优先**：医学循证、理财不荐股、关系不评判、健身不诊断
- **可迭代**：交付后提供深挖方向，支持多轮调研
- **可沉淀**：输出格式可直接存入个人知识库（Obsidian 等）

## 📝 使用示例

```text
用模板 9 帮我规划一次 5 天重庆→成都的旅行，预算 3000，情侣出行
用模板 1 帮我找 Obsidian 的同类笔记软件，要求本地免费
用模板 10 帮我做 10 万块钱 3 年期理财规划（只要框架，不荐具体产品）
```

详见 `examples/` 目录。

## 📄 许可证

MIT License。欢迎 fork、提交改进、分享使用。

## ⭐ 如果你觉得有用

点个 Star 就是最大的支持。欢迎提 Issue 建议新模板类型。
