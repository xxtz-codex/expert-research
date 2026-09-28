---
name: expert-research
description: "Expert-grade multi-type deep research and decision-support skill. 14 expert templates: tool/software alternative selection, learning path design, competitor analysis, local environment setup, content strategy, evidence-based medical consultation, resume/career optimization, purchase decision, travel planning, investment planning, home renovation material selection, life planning, relationship communication coaching, fitness training. Use when the user asks for similar solutions/alternatives ('find me X like Y'), deep research, expert-grade planning, analysis, or decision support - in Chinese or English. Each template includes expert workflow, hidden blind-spot dimensions, quality red lines, output format, and iteration follow-ups."
---
# Expert Research & Decision Support

This skill ships 14 expert-grade templates plus a fallback router. Pipeline: input parsing → type recognition → execute the matching template (Expert Workflow → Hidden Blind-Spot Dimensions → Quality Red Lines → Output Format → Iteration Follow-ups) → General Blind-Spot Checklist (optional deep mode) → Delivery Self-Check.

## Full Template Library (read first)

`references/prompt-template.en.md` is the complete v8 template library: the full text of all 14 templates, the fallback template, the 12-category general blind-spot checklist, the delivery self-check checklist, the knowledge-capture output format, and usage notes. Read it before executing, then run the template matching the user's problem type.

## Type Routing

| User problem type | Template |
|---|---|
| Tool/software alternative selection | Template 1 |
| Systematic learning of a skill/subject | Template 2 |
| Product/competitor analysis | Template 3 |
| Local environment/setup plan | Template 4 |
| Content creation topic selection | Template 5 |
| Health/medical consultation | Template 6 |
| Resume/job-hunt optimization | Template 7 |
| Consumer/purchase decision | Template 8 |
| Travel planning | Template 9 |
| Investment & financial planning | Template 10 |
| Renovation material selection | Template 11 |
| Life planning | Template 12 |
| Couple/relationship communication | Template 13 |
| Fitness training | Template 14 |
| Unclear type | Fallback template |

## Deep Mode

When the user says "deep" / "more comprehensive", additionally run through the 12-category general blind-spot checklist in `references/prompt-template.en.md`.

## Compliance Red Lines

Medicine: evidence-based only, no diagnosis, no prescriptions. Finance: framework only, not investment advice, no stock picks. Relationships: neutral and non-judgmental, no breakup assertions. Fitness: safety red lines, no injury diagnosis.

## Delivery Self-Check (before every delivery)

Source links are real and openable; every conclusion is marked ✅ verified / ⚠️ to verify / ❌ not found; facts separated from inference; blind-spot dimensions checked one by one; comparison tables carry a real comparison axis; nothing fabricated; trade-offs and costs stated; compliance notes for medicine / finance / relationships / fitness all present.

## Knowledge Capture

Use the knowledge-capture output format at the end of `references/prompt-template.en.md` to store conclusions into the user's knowledge base (e.g., Obsidian).
