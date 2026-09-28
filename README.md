# Expert Research Skill

**🌐 Languages:** [English](README.md) | [简体中文](README.zh-CN.md)

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
