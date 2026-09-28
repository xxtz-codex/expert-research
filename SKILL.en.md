---
name: expert-research
description: "(English version) Expert-grade multi-type deep research and decision-support skill. 14 expert templates: tool/software alternative selection, learning path design, competitor analysis, local environment setup, content strategy, evidence-based medical consultation, resume/career optimization, purchase decision, travel planning, investment planning, home renovation material selection, life planning, relationship communication coaching, fitness training. Use when the user asks for similar solutions/alternatives ('find me X like Y'), deep research, expert-grade planning, analysis, or decision support - in English or Chinese. Each template includes expert workflow, hidden blind-spot dimensions, quality red lines, output format, and iteration follow-ups."
---
# Expert Research & Decision Support

This skill ships with **14 expert templates** plus a fallback router. Flow: parse the input → identify the problem type → execute the matching template (Expert Workflow → Hidden Blind Spots → Quality Red Lines → Output Format → Iteration Follow-ups) → General Blind Spots (optional deep version) → Delivery Self-Check.

---
## Template 1 · Tool / Software Alternative Research (Technology Selection Expert)

**Role:** Senior technology selection and software evaluation expert.

```
Act as a technology selection expert and help me find alternatives to / substitutes for [X], and give a selection recommendation.

I. Full-ecosystem scan
1. Coverage channels: official ecosystem (plugin marketplace / extension store), GitHub (repo + stars + recent commits), community forums, channels accessible from China
2. Build a candidate pool: 10-15 candidates, covering three tiers (open source / free tier / paid), each with a source link

II. Initial screening (give screening conclusions, not a mere list)
Mark each candidate: ✅ verified / ⚠️ to verify / ❌ not found
- Free availability: open-source license (MIT/Apache/GPL…) or free-tier quota and limits
- Maintenance status: last commit date, star trend, issue response, whether it is close to abandonment
- Platform compatibility: native Windows support, version requirements

III. Deep review of 5-8 shortlisted candidates
1. Feature coverage comparison table: core features × candidates matrix (✓/✗/partial), highlight key differences
2. Performance and resource usage: startup/runtime overhead, large-file/large-data behavior (cite real benchmarks when available)
3. Onboarding cost: learning curve, documentation quality, community tutorial volume, Chinese localization
4. Extension ecosystem: plugins/API/integration capabilities (can it connect to my existing toolchain)
5. Privacy and data policy: whether data goes to cloud, whether it is used for training, quote exact clause text
6. License compliance: commercial-use limits, self-hosting limits, embedding limits

IV. Selection recommendation (the most important output)
- Give 2-3 recommended paths by scenario: best overall / lightest / most powerful, each with target user and trade-off
- Migration path: steps to move from [X] to a candidate, data-format compatibility, workflow impact
- Explicitly state which candidates are NOT recommended and why

V. Risk list
- Abandonment warning signs, free-to-paid traps, supply-chain security (maintainer reputation, dependency tree), privacy clauses quoted line by line

[Hidden Blind Spots] (points you haven't thought of that affect the decision — check each one)
1. Data lock-in: how hard is it to export/migrate data? Closed or open format?
2. License copyleft: GPL/LGPL/SSPL restrictions on commercial use and embedding — it's not just "free"
3. Security record: CVE history, security response speed, least-privilege permission model
4. Supply-chain single point: number of core maintainers (bus factor), acquisition/abandonment signals, dependencies of dependencies
5. Third-party ecosystem permissions: what plugins/extensions can read (API keys, files, clipboard)
6. Benchmark marketing: are official performance figures reproducible (real tests vs. marketing)
7. Free-tier lock-in path: does the free version deliberately create migration friction (incompatible formats, paid export)
8. Long-term cost: forced upgrades, cloud-feature dependency, maintenance effort
9. Migration cost measured for real: actually run export → import → verify, don't trust marketing (stuck migration = hidden lock-in)
10. Cold-start trap: candidate ecosystem too small → nobody answers questions, zero tutorials, no plugins
11. Dual-run cost: data synchronization and effort overhead while running both tools in parallel
12. Counter-example validation: actively look for complaints from people who "switched away from the candidate" — worth more than praise

[Quality Red Lines] (never cross)
1. Every candidate link must actually open (no unverified links from memory)
2. Comparison tables must have a real comparison axis (no list-style rambling)
3. Privacy clauses must be quoted verbatim (no paraphrasing or "reportedly")
4. Commercial/embedding use must state the license type (GPL/MIT/SSPL differences)
5. "Not recommended" must give a concrete reason (no vague "each has its merits")

[Output Format] (deliver in this structure, ready to use)
1. Candidate overview table: name | tier (open source/free/paid) | source link | status (✅/⚠️/❌) | one-line verdict
2. Deep-review comparison table: candidate | feature coverage | performance | onboarding | ecosystem | privacy | license
3. Recommendation paths: scenario → first choice → reason → trade-off
4. Risk list: risk item | evidence/source | mitigation

[Iteration Follow-ups] (offer after delivery, let me choose to dig deeper)
① Deep-dive review of one candidate? ② Migration walkthrough (export → import → verify)? ③ Alternatives under a different budget/permission? ④ A dedicated counter-example/complaint review of candidates?
```

---

## Template 2 · Systematic Learning Path (Learning Design Expert)

**Role:** Education planning and learning-path design expert.

```
Act as a learning-path design expert and systematically plan a learning program for [X].

I. Goal decomposition (set standards first)
- Split the goal into three levels: beginner (can independently complete basic tasks) → proficient (can independently complete full projects) → expert (can solve hard problems / teach)
- For each level, give: a verifiable capability standard + one deliverable artifact

II. Phased path (2-4 weeks per phase)
Each phase must include four parts:
1. Topic modules: what to learn this phase, why in this order (state prerequisite dependencies)
2. Required resources: authoritative textbooks (with version), official docs, courses (with links)
3. Practice tasks: 2-3 concrete executable tasks (with acceptance criteria)
4. Milestone check: phase test / mini project; how to catch up if you fail

III. Curated resources (all real and accessible, with links)
- Textbooks/books (mark version and timeliness), courses (platform + instructor), docs (official/community)
- Video tutorials (with links + knowledge-point summaries)
- Practice projects: 2-3 GitHub repos (mark difficulty and suitable phase)
- Communities: forums/Discord/groups/knowledge bases

IV. Pitfall guide
- Common misconceptions, how to spot outdated tutorials (check version/era), pacing advice, what can be skipped

V. Deliverables
- Learning roadmap (phased timeline), weekly plan table, resource list (grouped by phase)

[Hidden Blind Spots] (points you haven't thought of that affect learning outcomes)
1. Cognitive load: is the information volume per phase overloaded? Split into digestible units
2. Forgetting curve: schedule review points (review 1 day / 1 week / 1 month after learning), don't learn and dump
3. Path-dependency risk: "wrong paradigms" learned early are extremely expensive to fix later — prefer official/authoritative routes
4. Hidden cost of outdated material: learning from old versions means hitting every pitfall
5. AI-assistance boundary: which steps AI can accelerate (research, error fixing), which must be practiced yourself (core skills)
6. ROI curve: which phase pays back fastest, which phase is easy to quit — have a psychological plan
7. Portfolio value: can each phase's output go straight into a resume/portfolio
8. Resource hoarding trap: saving videos ≠ learning; require "hands-on verification" instead of "watched it"
9. Learning-loop check: only "output" counts as learned (teach others / write notes / build something); input-only learning is self-deception
10. Daily minimum viable amount: design a plan that advances in "30 minutes a day", avoiding the high restart cost after a break
11. Textbook-selection cost: authoritative textbook (slow but right) vs. popular tutorial (fast but shallow) — decide the mix and order

[Quality Red Lines] (never cross)
1. Resource links must really open (no vague "just search Baidu" directions)
2. Every level's goal must be verifiable (no unverifiable words like "understand/master/familiar")
3. Practice tasks must have acceptance criteria (how do you know you're done)
4. Tutorials/books must state version and timeliness (a 2020 tutorial must be flagged as possibly outdated)

[Output Format] (deliver in this structure)
1. Learning roadmap: phase → duration → goal → milestone deliverable
2. Phase detail table: each phase | modules | required resources (links) | practice tasks | pass criteria
3. Resource list: grouped by phase | type | name | link | version/timeliness
4. Pitfall list: misconception | consequence | correct approach

[Iteration Follow-ups] (offer after delivery)
① Refine a phase into weekly plans? ② Practical AI-assisted learning workflow? ③ Custom exercises for one deliverable (e.g. portfolio)? ④ A dedicated learning blocker & breakthrough session?
```

---

## Template 3 · Product / Competitor Analysis (Business Analyst)

**Role:** Senior business analyst / consultant.

```
Act as a business analysis expert and deeply analyze [X product] and its competitive landscape.

I. Competitor map (layered)
- Direct competitors (same category, same audience), indirect competitors (different form, same need), potential substitutes (new tech/new forms)
- For each: name, vendor, one-line positioning, source link

II. Deep comparison (shortlist 5-8, build a comparison table)
- Target audience and typical scenarios, core feature coverage (features × competitors matrix)
- Pricing: free tier / paid tier / hidden costs (storage, usage, seats) — use official pricing pages and cite sources
- Technical architecture and ecosystem: open API, integrations/plugins, data portability
- Regional availability: availability in China, filing/compliance status

III. Market landscape and trends
- Market size and growth (cite source and as-of date), leader share signals, funding/policy/regulatory moves
- Clearly separate: verified public data vs. analytical inference

IV. User insights (with evidence)
- Concentrated praise points, concentrated complaints (app stores/forums/social media, with links and dates)
- Typical user scenarios and word-of-mouth signals (net promoter, churn reasons)

V. Decision framework (if I'm choosing or migrating)
- Selection matrix: requirement weights × candidate scores (score and explain the rationale)
- Migration cost: data formats, export capability, team habits, workflow changes
- Switch risks and mitigation: downtime, data loss, learning cost

[Hidden Blind Spots] (points you haven't thought of that decide judgment quality)
1. Growth quality: real retention or burning money on vanity metrics (inflated DAU/subsidized users)
2. Financial signals: gross margin, customer acquisition cost, R&D investment share (cite sources for listed companies)
3. Ecosystem lock-in: do API/plugins/data create switching barriers, and how long are you locked
4. Price war & M&A risk: competitors may be acquired, raise prices, or shut down (historical signals)
5. Regulation and compliance: cross-border data, filing, industry access (AI products especially: generated-content compliance)
6. Founder/team signals: core team departures, open-source to closed-source, flip-flopping business direction
7. Users "registered but inactive": high signups but low activity — real usage depth matters more than numbers
8. Review manipulation: spotting astroturfing (review timestamp distribution, account patterns)
9. Pricing-strategy signals: history of free → paid moves (when did they start harvesting, are users locked in)
10. Marketing-case authenticity: case scale, verifiability, suspicion of "testimonials = own employees"
11. Exit cost measured for real: how long does a full data export take, is the format open

[Quality Red Lines] (never cross)
1. Market size/share and other data must carry a source and as-of date (no unsourced numbers)
2. Strictly separate "verified facts" from "analytical inference" (never mix)
3. User word-of-mouth must have evidence links (no "the internet says / many people say")
4. Financial signals of listed companies must cite filings/announcements

[Output Format] (deliver in this structure)
1. Competitor map: three columns — direct / indirect / potential
2. Deep comparison table: competitor | positioning | pricing | features | ecosystem | region
3. Market summary: size/trend/regulation (with source and date)
4. User insights: praise hotspots | complaint hotspots | evidence links
5. Decision matrix: requirement weights × candidate scores → conclusion and migration path

[Iteration Follow-ups] (offer after delivery)
① Deep-dive one competitor? ② A concrete migration execution checklist? ③ Personalized scoring for my usage scenario? ④ A dedicated churn-reason study of one competitor?
```

---
## Template 4 · Local Environment / Setup Plan (DevOps Expert)

**Role:** Senior ops/environment setup engineer.

```
Act as a senior environment engineer and help me [set up / configure X environment] on my computer.

I. Solution research (find existing solutions first)
- Prefer official installation methods (doc link + version requirements), ready-made GitHub solutions/one-click scripts (star count & update status), community best practices
- Mark each: ✅ verified / ⚠️ to verify, and explain why it was chosen

II. Pre-assessment (give conclusions before touching anything)
- Hardware and dependencies: based on my computer ({GPU / VRAM / RAM / disk}) give a feasibility verdict: sufficient / borderline (state where the bottleneck is) / insufficient (give an alternative path)
- Version compatibility matrix: software version × dependency version × my OS (Windows 11)
- Conflict check: conflicts with similar tools I already have (ports/drivers/environment variables)

III. Step-by-step implementation (directly executable)
- Environment prep → install → configure → verify; each step gives: the concrete command/action + expected output + what a failure looks like
- Windows-specific notes (paths, permissions, PATH, antivirus false positives)

IV. Failure playbook
- Common error quick-reference table: symptom → cause → fix (5-8 entries)
- Rollback plan: how to safely revert if the install breaks

V. Performance and security
- Tuning parameters, acceleration/cache options, daily maintenance
- Security baseline: default port exposure, key/credential storage, backup strategy

[Hidden Blind Spots] (points you haven't thought of that decide success or failure)
1. Driver/firmware/BIOS versions: GPU driver version directly affects CUDA/accelerator-stack behavior
2. Power and thermals: laptop plugged-in / discrete-GPU-direct / throttling strategies — check before heavy loads
3. Defender/antivirus interference: false-positive DLL deletion, script blocking — add exclusions before install
4. Environment variables and PATH pollution: multi-version conflicts (node/python/cuda coexisting)
5. Rollback point: record current versions before changes so you can revert on failure
6. Network proxy/mirrors: domestic download sources, pip/npm mirror config, avoid hanging forever
7. Windows Update interference: auto-updates can break drivers/runtime
8. Disk layout: C-drive space, which drive holds models/cache (big files stay off the system drive)
9. Hidden dependencies: compilers (MSVC), runtimes (VC++ Redistributable), privileges (admin)
10. Power plan and energy saving: laptop battery-saver mode causes sudden performance drops
11. Uninstall and leftovers: if you don't want it anymore, how to clean residual files/services/registry
12. Port conflicts: default ports colliding with other resident services (8080/3000/11434…), check occupancy first
13. Encoding and timezone: GBK vs UTF-8 in Chinese Windows environments, timezone affecting builds

[Quality Red Lines] (never cross)
1. Every step's command must give "expected output + failure symptom" (no commands without consequences)
2. Any change must have a rollback point (backup/version record/recoverable path)
3. Windows-specific pitfalls must be explicitly flagged (PATH/permissions/antivirus/encoding)
4. System-config changes must state the blast radius before executing

[Output Format] (deliver in this structure)
1. Feasibility report: hardware/dependencies | verdict (sufficient/borderline/insufficient) | bottleneck | alternative path
2. Implementation checklist: step | command/action | expected output | failure symptom
3. Error quick-reference: symptom | cause | fix
4. Security baseline: exposure | credentials | backup

[Iteration Follow-ups] (offer after delivery)
① Detailed troubleshooting for one step? ② A performance-tuning session? ③ Integrating with my existing toolchain? ④ Uninstall/cleanup leftover session?
```

---

## Template 5 · Content Creation Topics (Content Strategy Expert)

**Role:** Senior new-media editor / content strategy expert.

```
Act as a content strategy expert and help me plan content around [X topic].

I. Topic matrix (3-5 differentiated topics)
For each topic give:
- One-line angle, target audience, expected spread point (why it can go viral)
- Competition assessment: saturation of similar content, my differentiation
- 2-3 candidate titles (different styles: suspense / value-dense / emotional / controversial)

II. Viral-piece teardown (find 5-8 benchmarks, with links)
- Title formula, opening 3-second hook, content structure (sections/pacing), punchline position, ending CTA
- Extract one "reusable method" per piece — copying the content itself is forbidden

III. Platform strategy
- Algorithm/recommendation logic (current mechanism of that platform), best publishing windows, tag/cover/title rules
- Interaction design (comment/save/share triggers)

IV. Toolchain
- Script templates, recording/editing/voice/cover tools (recommend based on my computer config)

V. Landing deliverable (the most important output)
- Pick 1 best topic and deliver a ready-to-start outline: 3 title options + hook copy + section outline (key points per section) + ending CTA + image/cover plan

[Hidden Blind Spots] (points you haven't thought of that decide long-term account value)
1. Copyright and rewording red lines: licensing boundaries for music/fonts/images/film material — one lawsuit wipes everything
2. Platform banned words and industry red lines: medical exaggeration, financial inducement, superlative claims (especially reviews/science content)
3. Personal-info exposure: long-term privacy cost of showing your face/environment/data on video
4. Algorithm dependence and multi-platform distribution: single-platform traffic hostage, build a simultaneous distribution matrix
5. Traffic trap: buying views/mutual likes looks good short-term but damages account weight
6. Persona consistency: keep content style and stance consistent long-term; don't betray your persona for traffic
7. Comment and DM management: negative-news playbook, how to handle controversial follow-ups
8. Material reuse system: one production, multi-platform adaptation, lower marginal cost
9. Data review: how to read week-one data (completion rate/bounce/save ratio) to decide iteration
10. Monetization path in advance: how to monetize after growing (ads/knowledge products/affiliate) — don't wait for 100k followers
11. Platform red-line details: external-link rules (will posting WeChat/Taobao get you throttled), concrete banned-word lists
12. Capacity math: how many posts/videos can you really produce per week (declaring daily uploads without capacity always collapses)
13. Comment-section operations: pinned comment, curation rhythm, how to handle negative comments

[Quality Red Lines] (never cross)
1. Viral-piece teardowns must have real links (no memory-based summaries)
2. Titles don't overpromise: no titles promising what can't be delivered (clickbait backfires on weight)
3. Medical/financial/education content: no superlatives or outcome guarantees
4. No gray-industry operations: no rewording/copy-pasting/mass account farming

[Output Format] (deliver in this structure)
1. Topic matrix: topic | angle | audience | spread point | competition | candidate titles
2. Teardown table: benchmark | title formula | hook | structure | reusable method
3. Platform strategy: mechanism | timing | tag/cover rules | interaction design
4. Landing outline: 3 titles + hook copy + section points + CTA + cover plan

[Iteration Follow-ups] (offer after delivery)
① Write one topic into a full draft? ② Customize for one platform (Bilibili/Xiaohongshu/Douyin)? ③ Teardown more benchmarks? ④ Capacity & content calendar planning?
```

---

## Template 6 · Health / Medical Consultation (Evidence-Based Medicine Expert)

**Role:** Evidence-based medicine consultation — does not replace an in-person visit; provides evidence and healthcare navigation only.

```
[Symptom / report / medication question]:
Please handle it to evidence-based-medicine standards:
① Problem decomposition and information-limitation statement (what's missing, why it affects judgment)
② Authoritative basis: clinical guidelines / expert consensus / official textbooks (state evidence level and issuing body)
③ Care-seeking advice: when you must see a doctor, which department, how to prepare for the exam
④ Risk alerts: boundaries of self-care, danger signs (situations requiring immediate medical attention)
⑤ Source grading: ✅ guideline/authority / ⚠️ general science content / ❌ not found
Finally state clearly: content is for reference only, does not replace an in-person visit; if symptoms persist or worsen, seek medical care promptly.

[Hidden Blind Spots] (points patients/families often ignore that affect judgment)
1. Timeline details: when symptoms started, frequency, triggers — more important than "where it hurts"
2. Drug interactions: overlap risk between current medications/supplements and the suggested plan (including TCM)
3. History and family history: chronic disease, allergies, genetic factors affecting judgment
4. Reference ranges: the same lab value has different ranges across hospitals/ages/genders
5. Fake-science detection: common patterns in short-video/home-remedy/supplement pitches
6. Care timing window: which symptoms have a "golden hour" (chest pain / stroke / foreign-body aspiration)
7. Second opinion: get a re-check before major diagnoses
8. Cost and insurance: cost gradient of exams/treatments, avoid over-testing
9. Lab-sheet context: reference range ≠ clinical significance (borderline values need history/symptoms to interpret)
10. Special-population dosing: liver/kidney function, pregnancy/lactation, pediatric contraindication differences
11. Boundary of online diagnosis: AI/search can only point a direction, cannot replace physical exam and in-person visit

[Quality Red Lines] (never cross)
1. Basis must come from traceable evidence-based sources (guidelines/authorities/official textbooks); no marketing fluff
2. Never output a diagnosis or prescription under any circumstances
3. Must include "seek care if symptoms persist or worsen"
4. Danger signs (immediate-care situations) must be listed separately and prominently

[Output Format]
1. Information gaps: what's missing → what to supply
2. Evidence-based conclusion: point | evidence level | source
3. Care guidance: when to seek care | which department | exam prep
4. Danger signs: situations requiring immediate care (listed separately and prominently)

[Iteration Follow-ups] (offer after delivery)
① Reassess after you supply specific symptom details? ② Interpret one exam/report item? ③ A drug-interaction session? ④ Knowledge review of a condition (not personal diagnosis)?
```

---

## Template 7 · Resume / Job Search Optimization (Career Development Expert)

**Role:** Senior HR / career development expert.

```
Act as a career development expert and help me optimize [my resume / job-search plan].

I. Current-state diagnosis
- Score resume structure, highlight density, and match with the target role item by item; point out what most hurts the interview rate

II. Role benchmarking
- Deconstruct the target JD: keywords, hard skills, soft skills, hidden requirements (education/years/certs)
- Gap list: my experience vs. the JD

III. Resume rebuild (give per-module changes)
- Self-summary (one-line positioning), project experience (STAR + quantified outcomes), skill list (ordered by role), education/certs
- For each item, give a "before vs. after" example

IV. Job-search strategy
- Channel selection, application rhythm, follow-up scripts (templates), proactive outreach scripts

V. Interview prep
- Top-10 frequent questions (with my answering framework), 30s/60s self-intro versions, questions to ask at the end

[Hidden Blind Spots] (points you haven't thought of that affect outcomes)
1. ATS parsing compatibility: layout/keywords/file format (PDF vs Word) — does it pass machine screening
2. Authenticity and reference checks: no fabrication/inflation; quantification must be real and explainable
3. Salary negotiation strategy: basis for your range, option/performance valuation, raise benchmarks
4. Framing gaps/career changes/frequent job hops
5. Persona consistency: resume, portfolio, interview performance, and reference-check story must fully match
6. Quantification authenticity: use real relative growth, not invented numbers
7. Handling objective constraints: common doubts about age/region/education/late career changes and responses
8. Leaving-reason framing: consistent with references and former colleagues
9. Resume density and layout: one page or two, keyword density, machine readability (no images/fancy layouts)
10. Keyword-match self-check: line up JD keywords against the resume word by word; if coverage is low, add them
11. Channel strategy: referral > headhunter > direct apply > mass apply (effectiveness varies); separate big-company vs. small-company strategy

[Quality Red Lines] (never cross)
1. No fabricated experience, positions, or numbers (all quantification must have real basis)
2. Rebuild examples must give "before vs. after" (no abstract advice only)
3. Interview answers give a framework, not fabricated lies that backfire
4. Reference-check/leaving-reason framing must be honest and consistent (no lying scripts)

[Output Format]
1. Diagnosis report: issue | impact | priority
2. Rebuilt resume: a paste-ready version per module
3. Interview bank: question | answering framework | my version example

[Iteration Follow-ups] (offer after delivery)
① Customize for a specific role's JD? ② Salary negotiation simulation? ③ Career-change / employment-gap session? ④ Portfolio/project-experience packaging session (on a truthful basis)?
```

---
## Template 8 · Purchase / Shopping Decision (Rational Consumer Advisor)

**Role:** Rational consumer advisor (knows markets, specs, and marketing tricks).

```
Act as a rational consumer advisor and help me make the purchase decision for [X].

I. Need clarification
- Real need vs. want: usage frequency, scenarios, pain points, budget range
- One-line decision criterion (e.g. performance-first / portability-first / value-first)

II. Candidate comparison (3-5)
- Price (official/historical/channel price), core specs, word of mouth (with sources), pros and cons

III. Value analysis
- Lifecycle cost: consumables, upgrades, accessories, repairs, depreciation speed
- Value per yuan comparison

IV. Purchase timing
- Discount patterns (618/Double-11/product cycles), fake-promotion detection (raise-then-discount), whether it's worth waiting

V. Decision conclusion
- Buy / don't buy / wait — with reasons + alternatives + regret-cost assessment

[Hidden Blind Spots] (points you haven't thought of that affect the decision)
1. Marketing-trick recognition: price anchors, scarcity scripts, sponsored reviews, review-for-cashback
2. Hidden costs: consumables, subscriptions, accessories, repairs, electricity
3. Warranty and after-sales: policy, service network, replacement conditions
4. Second-hand / refurbished / factory-refurbished value and risk
5. Ecosystem lock-in: accessories, accounts, data, charging protocols
6. Safety compliance: 3C certification, battery safety, radiation standards
7. Needs-change risk: buy and never use / novelty fading
8. Sunk cost and upgrade temptation: overspending to complete bundles or "upgrade"
9. Historical price curve: use price-trackers to see 3-6 month trends, spot "raise-then-discount" fake sales
10. Review credibility filtering: read follow-up reviews / mid-to-negative reviews / buyer photos; watch for all-identical praise and instantly deleted complaints
11. Try before you buy: test/borrow/rent when possible (especially large or expensive items)

[Quality Red Lines] (never cross)
1. Prices must carry a source and query time (no made-up quotes)
2. Products without 3C/safety certification must carry a risk warning (no endorsing uncertified products)
3. The conclusion must be one of "buy / don't buy / wait" + reason (no vague "depends on your needs")
4. No inducing over-borrowing / installment impulse (rational boundary)

[Output Format]
1. Need-clarification table: need | frequency | scenario | budget | decision criterion
2. Candidate comparison table: candidate | price | specs | word of mouth | pros and cons
3. Decision conclusion: buy/don't buy/wait | reason | alternative | regret cost

[Iteration Follow-ups] (offer after delivery)
① Deep review of one candidate? ② Better options within budget? ③ Second-hand/channel price comparison? ④ Historical price and purchase-timing analysis?
```

---

## Template 9 · Travel Planning (Travel Planner)

**Role:** Senior travel planner (knows destinations, pacing, budget, and risk).

```
Act as a senior travel planner and help me plan [X destination / itinerary].

I. Need clarification
- Trip days, budget range, companions (elderly/kids/solo), pacing preference (military vs. relaxed)
- Must-see list and "can be dropped" list

II. Itinerary framework
- Day allocation (cities/scenic areas), route logic (don't backtrack), transport connections
- Season and weather judgment: suitable this time? alternatives

III. Day-by-day itinerary
- Each day: morning/afternoon/evening plans, attraction opening hours, reservation requirements
- Food/accommodation area suggestions, daily transport
- Plan B: weather / energy / closed-day alternatives

IV. Budget breakdown
- Five categories: transport/accommodation/tickets/food/shopping, total and savings (what can be cut)

V. Pre-trip checklist
- Documents and visas, reservation confirmations, packing list, insurance, emergency plan (embassy/hospital/police numbers)

[Hidden Blind Spots] (points you haven't thought of that decide trip quality)
1. Seasonal risks: typhoons, rainy season, peak crowds, high-altitude reactions
2. Visa and entry policy: validity, materials, rejection rate, visa-on-arrival vs. e-visa
3. Hidden costs: in-scenic-area transport, peak-season premiums, shopping-kickback traps, tipping rules
4. Safety risks: crime zones, scam patterns (taxis/currency exchange), insurance coverage
5. Transport connection gaps: minimum transfer time, last train/ferry, rush-hour congestion
6. Companion needs: elderly stamina, kids' food, medical accessibility
7. Local customs and compliance: dress, photography, religious taboos, drone/filming restrictions
8. Itinerary slack: over-packed schedules always collapse; keep flex time daily
9. Exchange rates and payment: cash/credit/mobile-payment coverage, foreign ATM fees
10. Insurance claim essentials: exclusions (pre-existing conditions/extreme sports), reporting deadlines
11. Document backup: electronic + paper copies of entry documents (plan for losing your passport)

[Quality Red Lines] (never cross)
1. Volatile info (opening hours/reservation requirements/ticket prices) marked "check official sources for latest" (no permanent-accuracy claims)
2. Safety warnings are mandatory (crime areas/weather disasters/high-risk activities)
3. Budget tables must be executable (line items with basis, no inflated numbers)
4. High-risk activities (diving/skydiving/self-driving) must flag insurance and qualification requirements

[Output Format]
1. Itinerary overview: date | city/area | theme | transport | accommodation area
2. Day-by-day detail: time slot | arrangement | reservation needs | alternative
3. Budget table: category | estimate | what can be cut
4. Pre-trip checklist: documents | bookings | packing | insurance | emergency numbers

[Iteration Follow-ups] (offer after delivery)
① Detail one day further? ② A budget-compression plan? ③ Accommodation area/hotel recommendations? ④ Weather/holiday risk reassessment?
```

---

## Template 10 · Investment Planning (Financial Planning Advisor)

**Role:** Financial planning advisor. ⚠️ Compliance red lines: no guaranteed returns, not investment advice, risk is yours; all product info subject to official/regulatory disclosures.

```
Act as a financial planning advisor (compliant, not investment advice) and help me with [financial goal / money planning].

I. Financial snapshot
- Income/expenses/balance, assets/liabilities/cash flow, monthly investable amount

II. Goals and risk assessment
- Financial goals (horizon: short/mid/long term), target amount, liquidity needs (when will you need the money)
- Risk tolerance: maximum drawdown you can bear, investing experience

III. Allocation framework (framework ratios only, no specific picks)
- Major-asset-class allocation suggestion: cash/emergency fund, stable (low volatility), aggressive (high volatility) — how much each
- Tool types per class (deposits/money-market funds/bonds/index funds, etc.), with risk level and liquidity

IV. Product comparison (compare within the same class, no cross-class picks)
- 3-5 same-type products compared: fees, minimums, liquidity, historical volatility (cite sources)
- Explicitly state: historical performance ≠ future returns

V. Pitfall avoidance and discipline
- Common scam recognition (high interest / pig-butchering / MLM / crypto pitches)
- Long-term impact of chasing highs, panic selling, and fee erosion
- Dollar-cost-averaging / position discipline suggestions

[Hidden Blind Spots] (points you haven't thought of that affect outcomes)
1. Emergency fund first: cover 3-6 months of expenses before investing
2. Debt cost vs. investment return: pay off high-interest debt first
3. Fee compounding: management/purchase fees erode returns over time
4. Liquidity trap: lock-up periods/redemption limits/early-withdrawal penalties
5. Insurance gap: basic critical-illness/medical/accident coverage before investing
6. Inflation erosion: pure cash/deposits lose purchasing power long-term
7. Scams and pig-butchering: treat any "guaranteed high return" as fraud
8. Tax and compliance: tax on gains, account compliance
9. Psychological biases: chasing highs, loss aversion, herd behavior
10. Diversification and correlation: don't put all money into assets that rise and fall together (looks diversified, actually one risk)
11. Discipline rules: DCA rhythm, take-profit/stop-loss lines, add-position conditions — set rules before entering
12. Household view: don't just stare at one return; look at the household balance sheet and cash flow as a whole

[Quality Red Lines] (never cross)
1. Every output ends with a mandatory disclaimer: "not investment advice; markets carry risk"
2. No specific stocks/coins/tickers (only tool types and frameworks)
3. Historical performance/returns must be marked "≠ future returns"
4. Any "guaranteed high return" claim is flagged as a fraud red flag
5. Leverage / borrowed-money investing gets a strong warning

[Output Format]
1. Financial snapshot: income | expenses | assets | liabilities | investable amount
2. Risk assessment verdict: risk level + rationale
3. Allocation framework: asset class | ratio | tool types | risk level | liquidity
4. Product comparison table: product | fees | minimum | liquidity | historical volatility | source
5. Pitfall list: pattern | recognition signals | correct approach

[Iteration Follow-ups] (offer after delivery)
① Compare specific products? ② A dedicated goal session (house/retirement/education fund)? ③ Risk-tolerance reassessment? ④ A household financial check-up?
```

---

## Template 11 · Home Renovation & Material Selection (Home Improvement Advisor)

**Role:** Senior home renovation / building-materials advisor (knows materials, workmanship, budget, and traps).

```
Act as a senior home-improvement advisor and help me plan the renovation and material selection for [X layout / space].

I. Needs and budget
- Layout area, style preference, total budget, priority order (looks/durability/eco/saving)
- Per-square-meter budget reference and allocation direction

II. Space breakdown
- Material and workmanship differences per space (living/bedroom/kitchen/bathroom/balcony)
- High-frequency vs. low-frequency spaces, budget-allocation tilt

III. Main-material comparison (3-5 candidates per category)
- Flooring/tiles/wall paint/cabinets/doors/windows/countertops: price tiers, eco ratings, durability, construction difficulty
- Three-tier choices per category: comfortable budget / moderate / tight

IV. Auxiliary materials and hidden work (where you must not save)
- Plumbing/electrical materials, waterproofing, putty, adhesives, silicone — why auxiliary materials decide lifespan and eco-friendliness

V. Construction and acceptance
- Timeline estimate, key acceptance checkpoints (plumbing/electrical/waterproofing/tiling/painting)
- Change-order trap recognition and contract notes

[Hidden Blind Spots] (points you haven't thought of that decide renovation success)
1. Eco ratings: formaldehyde release (E0/ENF), board vs. solid wood, ventilation period
2. Hidden-work aftermath: waterproofing/electrical rework costs double
3. Change-order tricks: low-ball opening, material substitution, omitted items
4. Real pollution culprits: adhesives/putty/silicone/MDF — more toxic than wall paint
5. Waste and restocking: tile/flooring waste rates, batch color differences, discontinued-stock risk
6. Hardware/accessory long-term cost: hinges/faucets/switches — hard to replace when broken
7. After-sales and warranty: warranty years, verbal promises vs. contract
8. Seasonal construction: paint/tile hollowing, winter putty drying
9. Network and smart-home pre-wiring: outlets/network/smart-home points planned in advance
10. Budget buffer: keep 15-20% contingency, don't run at 100%
11. Contract and payment milestones: pay by phase (materials on site / hidden-work acceptance / completion), never pay all upfront
12. Measure the space first: a one-centimeter error wrecks the whole plan; measure/inspect precisely before work starts
13. Lighting and traffic lines: design main lights/spotlights/switch positions around how you actually live, before you regret it

[Quality Red Lines] (never cross)
1. Eco ratings must be explicit (E0/ENF/no label = risk warning)
2. Hidden-work (plumbing/electrical/waterproofing) acceptance checkpoints must be listed (top rework area)
3. Budget must include a buffer (never pinned at 100%)
4. No "save where you can" advice on safety items (waterproofing/circuits/load-bearing)
5. Material prices/brand info carry sources or "check local market" notes

[Output Format]
1. Budget allocation: space/item | budget | share
2. Main-material comparison: category | candidates | price | eco | durability | construction difficulty
3. Hidden-work list: item | material standard | acceptance point
4. Acceptance checkpoint table: phase | check item | pass criteria
5. Pitfall list: trick | recognition | countermeasure

[Iteration Follow-ups] (offer after delivery)
① A dedicated space session? ② Deep comparison of one main material? ③ A budget-adjustment plan? ④ A contractor vetting / anti-trap guide?
```

---
## Template 12 · Life Planning (Life Planning Coach)

**Role:** Life planning coach / career advisor (neutral, systematic, executable).

```
Act as a life planning coach and help me make a life plan for [phase / direction].

I. Current-state inventory
- Current phase, core resources (time/money/skills/network/health), main contradiction (the one thing you most want to solve)

II. Goal system (SMART-ified)
- Long-term (5 years) / mid-term (1 year) / short-term (90 days) — three layers
- Each goal: measurable, with a deadline, with acceptance criteria

III. Path design
- Goal → key paths (2-3 main lines) → milestones → checkpoints (how often to review)
- Dependency conditions and prerequisite skills per path

IV. Resource allocation
- How to allocate time/money/energy; explicitly state what you give up (trade-offs matter more than additions)

V. Risk and resilience
- Plan B, contingency buffers (money/time slack), reversible vs. irreversible decision list

[Hidden Blind Spots] (points you haven't thought of that decide whether the plan succeeds)
1. Reversibility check: are major decisions (house/career change/marriage/settling) reversible, and how costly is reversal
2. Opportunity cost: the explicit price of choosing A over B — write it down, don't gloss over it
3. Sunk cost: don't be held hostage by what you've already invested; stop-loss when needed
4. Compounding mindset: which skills/network/health/assets compound long-term, and deserve early investment
5. Energy management: you only have so much effective energy per day — allocation matters more than the schedule
6. Antifragility: buffer reserves, multiple income sources, transferable skills
7. Values calibration: is the goal what you truly want, or the "social clock" (everyone else is doing it)
8. Health and relationship floor: don't trade your body and key relationships for goals — that loss is irreversible
9. 90-day validation: run a 90-day experiment on big goals before going all in
10. Review mechanism: a plan without regular reviews is just a wish
11. Trial-cost math: the minimum verifiable experiment per option (cost/duration), small steps first
12. Environment leverage: city/industry/community choices > individual effort (compounding of platform and environment)
13. Financial-independence baseline: how much principal covers basic expenses from passive income — a long-term anchor

[Quality Red Lines] (never cross)
1. No single-value preaching (respect diverse definitions of "success"; don't judge the user's choices)
2. Goals must be measurable with deadlines (no empty goals like "live better")
3. Major decisions must include reversibility analysis (reversible vs. irreversible, reversal cost)
4. Mental-health signals (depression/self-harm signs): recommend professional help rather than only planning

[Output Format]
1. Current-state inventory: resource | status | gap
2. Goal tree: long-term → mid-term → short-term (90 days), each with acceptance criteria
3. Path map: goal → main line → milestone → checkpoint
4. Resource allocation: resource | allocation | what you give up
5. Risk table: risk | probability/impact | Plan B

[Iteration Follow-ups] (offer after delivery)
① Turn one goal into a 90-day action checklist? ② Major-decision assessment (house/career change)? ③ Values/priority calibration conversation? ④ Minimum trial-experiment design?
```

---

## Template 13 · Relationship / Couples Analysis (Relationship Communication Coach)

**Role:** Relationship communication coach. ⚠️ Boundaries: neutral and non-judgmental, never asserts "should you break up", respects personal choice, suggests professional counseling when needed (psychology / couples therapy).

```
Act as a relationship communication coach (neutral, non-judgmental) and help me sort out [the issue in my couple/intimate relationship].

I. Relationship status
- Interaction patterns, development stage, each side's core needs, the full story of the latest conflict (trigger/process/outcome)

II. Conflict decomposition
- Surface issue → deeper needs (of each side) → where each side's view is reasonable
- Pattern recognition: does the same pattern keep recurring

III. Communication plan
- Nonviolent-communication expression template (observation/feeling/need/request)
- Timing and approach (pause at emotional peaks, agree on a cooldown)
- Concrete script examples (before/after rewording)

IV. Relationship building
- Emotional bank account: accumulate positive interactions daily (validation/companionship/small surprises)
- Boundary setting: which are each side's own boundaries, which need negotiation
- Shared activities and novelty maintenance

V. Decision support (only when major decisions are involved)
- If it involves long-distance/meeting parents/moving in/breaking up: give a "decision framework" (needs list, negotiable items, bottom lines) — don't decide for the user

[Hidden Blind Spots] (points you haven't thought of that affect relationship quality)
1. Love-language differences: people express love differently (affirmation/companionship/gifts/service/touch) — mismatch causes misreading
2. Emotional triggers: sensitive points from family of origin and past trauma — not aimed at you
3. Communication timing: talking at emotional peaks always explodes; pause → cool down → agree to talk later
4. Boundaries and selfhood: healthy relationships don't require abandoning yourself; over-accommodation is unsustainable
5. Relationship risk signals: silent treatment/manipulation/belittling/control — be alert, seek professional help when needed
6. Expectation management: movie expectations vs. real relationships; lower unrealistic expectations
7. Third-party perspective: it's hard to see clearly from inside; friends or counselors give an outside view
8. Emotional deposits: the positive-interaction balance decides how fast conflicts repair
9. Repair actions: concrete apology/listening/behavior change, not empty words
10. Stage assessment: honeymoon vs. stable vs. burnout phases have different problems (stage mismatch is also a conflict source)
11. "I-statements": use "I feel…" instead of "you always…", reduces defensiveness
12. When to see a professional: repeated same-pattern conflicts / broken trust / major trauma — suggest couples counseling or individual therapy

[Quality Red Lines] (never cross)
1. Stay neutral: no judging who is right or wrong, no "should you break up" assertions
2. Never make decisions for the user (break up/get back together/compromise) — only decision frameworks
3. Control/violence/harm signals: clearly recommend professional help and safety first
4. No manipulation scripts (guiding/manipulating/playing games)

[Output Format]
1. Status overview: patterns | needs | development stage
2. Conflict decomposition: surface issue | each side's deeper needs | each side's valid points | recurring pattern
3. Communication scripts: scenario | old wording | new wording (NVC)
4. Action list: short-term (this week) | mid-term (this month) | boundaries and bottom lines

[Iteration Follow-ups] (offer after delivery)
① Communication simulation for a specific conflict? ② Long-distance/meeting-parents/cohabitation session? ③ A de-escalation plan for escalating conflicts? ④ Stage assessment and expectation calibration?
```

---

## Template 14 · Fitness Training (Exercise Science Expert)

**Role:** Exercise science / conditioning expert. ⚠️ Safety boundaries: doesn't replace a doctor; injuries/chronic conditions first consult a doctor; stop at pain.

```
Act as an exercise science expert and help me design a training program for [fat loss / muscle gain / conditioning / rehab].

I. Physical baseline
- Height/weight/body fat (if known), training background (what you've done / how long since), injury history (knee/back/shoulder…)
- Make the goal concrete: fat loss (target weight/body fat) / muscle gain (target body parts) / conditioning (running distance/pull-up count)…

II. Goal setting (safety standards)
- Safe-rate red lines: fat loss ≤ 0.5-1% body weight per week; monthly muscle growth has an upper limit — no quick-fix promises
- Cycle: 12 weeks per training cycle, checkpoints at weeks 4/8/12

III. Training plan (weekly framework)
- Weekly schedule: strength X days + cardio/recovery X days + rest X days (progress gradually, don't max out week one)
- Exercise library: by body part (push/pull/legs/core), with target and common mistakes
- Progressive overload: how to progress weight/reps/sets, what signals to add load

IV. Nutrition (aligned with goals)
- Calorie math: maintenance → fat-loss deficit / muscle-gain surplus (formula + examples; no meal replacements, no extremes)
- Protein needs: estimate by body weight (g/kg), food sources
- Three-meal template: breakfast/lunch/dinner + pre/post-workout eating

V. Execution and monitoring
- Training-log template (exercise/weight/reps/feeling)
- Progress checks: photos/measurements/strength, once a week — don't only watch the scale
- Plateau handling: when to change the plan and how

VI. Safety boundaries
- Form over weight (light but correct)
- Pain warnings: which pain means stop, which pain means see a doctor
- Rest and sleep: muscles grow during recovery; insufficient sleep wastes training

[Hidden Blind Spots] (points you haven't thought of that decide results and safety)
1. Injury history and contraindicated movements: knee injuries skip squat jumps / back injuries be careful with deadlifts — ask first, then prescribe
2. Progressive overload: not "train harder and harder" but systematic progression, or you WILL get hurt
3. Recovery and sleep: muscles grow during rest; training is the stimulus, recovery is the growth
4. Oversized calorie deficit side effects: metabolic slowdown, muscle loss, menstrual disruption, binge rebound
5. Supplement tax: beyond protein powder/creatine, 90% is marketing — nail the basic diet first
6. Movement compensation and joint stress: the body cheats (lower-back compensation/shrugging); beginners learn standard form with light weights
7. Plateau psychology and sustainability: short-term extreme plans always rebound; the plan must be sustainable for a year
8. Physical exam before training: sedentary/overweight/chronic conditions — get checked first, especially cardiovascular
9. Personalization: don't copy influencer plans (training level/recovery capacity/time budget all differ)
10. Sedentary special cases: tight hip flexors/rounded shoulders — do mobility work before intensity

[Quality Red Lines] (never cross)
1. No medical diagnosis (pain-cause judgment is for doctors); general safety principles only
2. No promised outcome numbers ("lose 20 jin in a month" is always flagged unhealthy/dangerous)
3. Pain principle: acute pain stops immediately, persistent pain sees a doctor
4. No extreme diets (fasting/single-food/over-reliance on meal replacements)
5. Training volume progresses gradually; week-one plan must be clearly below safety limits

[Output Format]
1. Physical baseline: data | training background | injury history | goal
2. Weekly training table: day | content | intensity | notes
3. Exercise list: exercise | target muscles | common mistakes | substitute
4. Nutrition template: meal | example content | calorie estimate
5. Monitoring table: week | weight/measurements/strength | adjustments

[Iteration Follow-ups] (offer after delivery)
① A dedicated body-part session (glutes/back/core)? ② Nutrition detail (delivery-food/student)? ③ Plateau breaking? ④ Training adjustments during injury rehab?
```

---

## Fallback Template · When the Type Is Unclear

```
Help me do deep research on [X]: first identify which category it belongs to (tool selection / learning plan / competitor analysis / environment setup / content planning / medical consultation / job-search optimization / purchase decision / travel planning / investment planning / renovation material selection / life planning / relationship analysis / fitness training / other),
then give a research plan to expert standards based on the type; after I confirm, execute (alternatives/similar items, resources, tutorials, blind spots — each item with source link + ✅/⚠️/❌).
```

---

## General Blind-Spot Checklist (append to any template as the "deep version" switch)

> Append this line to any template to enable:
> `Deep: deep version (append the general blind-spot checklist)`

**General blind-spot checklist (check each one; cite when present, otherwise note "no obvious risk found")**
1. **Cost blind spot**: hidden costs of free/cheap options (migration, data export, time, labor)
2. **Compliance blind spot**: licenses, data compliance (PIPL/GDPR), platform terms, industry access
3. **Privacy blind spot**: where data goes, whether it trains models, third-party sharing, human review
4. **Supply-chain blind spot**: dependency tree, single maintainer, acquisition/abandonment signals
5. **Security blind spot**: vulnerability history, permission model, attack surface
6. **Decision bias**: sunk cost (invested already ≠ reason to continue), confirmation bias (only looking for supporting evidence), trend trap (popular ≠ right for me)
7. **Long-term evolution**: maintainability, portability, ecosystem direction in 2-3 years
8. **Time blind spot**: how much time does this plan cost? Is there a faster path? Time cost is usually ignored
9. **Counter-example blind spot**: actively seek opposing evidence (negative reviews/failure cases/rant posts), not just supporting evidence
10. **Second-hand evidence blind spot**: distinguish primary data (official/measured) from secondary retelling (blogs/short-video reuploads); trace secondary claims to the source
11. **Opportunity-cost blind spot**: if you pick A, what do you give up? Write the forgone B down explicitly
12. **Verifiability blind spot**: can the key conclusions be tested/reproduced? Unverifiable "conclusions" downgrade to "opinions"

---

## Delivery Self-Check (AI self-audits before every delivery; fix first, then deliver)

1. Does every conclusion carry a source link? Do the links actually open?
2. Is every item marked ✅ verified / ⚠️ to verify / ❌ not found?
3. Are facts strictly separated from inference?
4. For computer-fitness items, is it marked installable / viewable / needs-config?
5. Are the [Hidden Blind Spots] checked one by one (cite evidence when present, note otherwise)?
6. Do comparison tables have a real comparison axis (not a list)?
7. Any fabricated data, features, reviews, or links?
8. Is there an executable next-step suggestion?
9. Is the output delivered in the template's [Output Format]?
10. Medical: evidence-based process + see-a-doctor note? Finance: "not investment advice"? Relationships: neutral, non-judgmental? Fitness: safety red lines?
11. Do the hidden blind spots exceed the user's awareness (showing "what you didn't think of")? At least 3 that the user probably didn't think of?
12. Are trade-offs and costs stated (not "everything is great" — what does choosing it cost)?

---

## Storable Output Format (optional after research, handy for Obsidian / knowledge base)

```
## Research Note: {topic}
- **Date**: {date} ｜ **Verdict**: {one line}
- **Candidate/key-point list**: name + source link + status(✅/⚠️/❌)
- **Decision advice**: choose/not + reason + trade-off
- **Blind-spot record**: privacy/compliance/cost/security… (when present)
- **To-verify items**: ⚠️ list (next update)
- **Iteration direction**: {the follow-up option chosen from the template}
```

---

## Usage Notes

- Pick template 1-14 by problem type; use the fallback router when unsure
- Each template already includes: expert workflow + hidden blind spots + quality red lines + output format + iteration follow-ups
- For deeper analysis, append: `Deep: deep version (append the general blind-spot checklist)`
- All templates share: traceable sources (link + ✅/⚠️/❌), public compliant channels only, read primary sources for key mechanisms, separate facts from inference
- Templates 1 and 4 inspect the computer only when "locally installable/usable" matters; other types don't
- Template 6 follows the evidence-based medicine flow; template 10 carries investment-risk disclaimers; template 13 stays neutral and non-judgmental; template 14 carries exercise safety red lines
- After research, use the [Storable Output Format] to save conclusions into your knowledge base

