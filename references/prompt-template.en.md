# Expert Research & Decision Support

This skill ships with 14 expert templates plus a fallback router. Pipeline: input parsing → type recognition → execute the matching template (Expert Workflow → Hidden Blind-Spot Dimensions → Quality Red Lines → Output Format → Iteration Follow-ups) → General Blind-Spot Checklist (optional deep mode) → Delivery Self-Check.

---
## Template 1 · Tool/Software Alternative Research (Technical Selection Expert)

[Role] Senior technical selection and software evaluation expert.

```
Using the standard of a technical selection expert, help me find alternatives/similar tools to [X] and give a selection recommendation.

1. Full-ecosystem scan
1. Coverage channels: official ecosystem (plugin market / extension registry), GitHub (repo + stars + recent commits), community forums, channels accessible from mainland China
2. Build a candidate pool: 10-15 candidates across three tiers — open-source / free tier / paid — with a source link for each

2. Initial screening (give a verdict per candidate, do not just list them)
Tag each candidate: ✅ verified / ⚠️ to be verified / ❌ not found
- Free usability: open-source license (MIT/Apache/GPL…) or free-tier quota and limits
- Maintenance status: last commit time, star trend, issue responsiveness, risk of being abandoned
- Platform compatibility: native usability on Windows, version requirements

3. Deep review of the shortlisted 5-8
1. Feature coverage comparison table: core features × candidates matrix (✓/✗/partial), flag key differences
2. Performance and resource footprint: startup/runtime overhead, behavior on large files/large datasets (cite sources for any measured numbers)
3. Onboarding cost: learning curve, documentation quality, volume of community tutorials, level of Chinese localization
4. Extension ecosystem: plugins/APIs/integration capability (can it plug into my existing toolchain?)
5. Privacy and data policy: does data leave the device/cloud, is it used for training, quote the relevant terms verbatim
6. License compliance: commercial-use restrictions, self-hosting restrictions, embedding restrictions

4. Selection recommendation (the most important output)
- Give 2-3 recommended paths by scenario: best overall / lightest / most powerful — state the target user and the tradeoff for each
- Migration path: steps to move from [X] to the chosen candidate, data-format compatibility, workflow impact
- Explicitly name candidates you "do not recommend" and why

5. Risk list
- Signals of impending abandonment, free-to-paid traps, supply-chain security (maintainer reputation, dependency tree), point-by-point citation of privacy terms

[Hidden Blind-Spot Dimensions] (points you did not think of but that affect the decision — check each one)
1. Data lock-in: how hard is it to export/migrate your data? Is the format closed or open?
2. License copyleft reach: what GPL/LGPL/SSPL actually restrict for commercial use and embedding — it is not just "free"
3. Security track record: CVE history, security response speed, whether the permission model is least-privilege
4. Supply-chain single point of failure: core maintainer count (bus factor), acquisition/shutdown signals, dependencies of dependencies
5. Third-party ecosystem permissions: what can plugins/extensions actually read (API keys, files, clipboard)
6. Benchmark marketing: are the vendor's performance numbers reproducible (real reviews vs. marketing)
7. Free-tier lock-in path: does the free version deliberately create migration friction (incompatible formats, paid export)
8. Long-term cost: forced upgrades, cloud-only features, maintenance headcount
9. Real migration trial: actually walk through export → import → verify; do not trust marketing (a stalled migration = hidden lock-in)
10. Cold-start trap: a candidate with too small an ecosystem → unanswered questions, zero tutorials, no one writing plugins
11. Dual-running cost: data sync and mental overhead of running two tools in parallel
12. Counter-example validation: actively seek negative reviews from people who tried the candidate and switched away — worth more than praise

[Quality Red Lines] (hard limits)
1. Every candidate link must actually open (no recommending unverified links from memory)
2. Comparison tables must have comparison axes (no laundry-list dumps)
3. Privacy terms must quote the key sentences verbatim (no paraphrase, no "reportedly")
4. Any commercial/embedding use must state the license type (GPL vs MIT vs SSPL differences)
5. "Do not recommend" must give a concrete reason (no vague "each has its strengths")

[Output Format] (deliver in this structure, ready to use)
1. Candidate overview table: Name | Tier (open-source/free/paid) | Source link | Status (✅/⚠️/❌) | One-line verdict
2. Deep-review comparison table: Candidate | Feature coverage | Performance | Onboarding | Ecosystem | Privacy | License
3. Recommended paths: Scenario → Top pick → Reason → Tradeoff
4. Risk list: Risk item | Evidence/source | Mitigation

[Iteration Follow-ups] (offer proactively after delivery so I can choose what to dig into)
① Deep-dive review of a specific candidate? ② Hands-on migration steps (export → import → verify)? ③ Alternatives if budget/permissions change? ④ A focused deep-dive on counter-example negative reviews for a candidate?
```

---

## Template 2 · Systematic Learning of a Skill/Subject (Learning-Path Design Expert)

[Role] Education planning and learning-path design expert.

```
Using the standard of a learning-path design expert, help me systematically plan a learning program for [X].

1. Goal decomposition (set the standard first)
- Split the goal into three levels: beginner (can independently complete basic tasks) → proficient (can independently deliver a full project) → master (can solve hard problems / teach others)
- For each level, give: a verifiable competency standard + one deliverable artifact

2. Staged path (2-4 weeks per stage)
Each stage must include all four pieces:
1. Topic modules: what to learn in this stage and why this order (state prerequisites)
2. Required resources: authoritative textbooks (note edition), official docs, courses (with links)
3. Practice tasks: 2-3 concrete, executable tasks (with acceptance criteria)
4. Milestone check: stage test / mini project, and how to remediate if it is not passed

3. Curated resources (all real and accessible, with links)
- Textbooks/books (mark edition and freshness), courses (platform + instructor), docs (official/community)
- Video tutorials (Bilibili and similar, with link + knowledge-point summary)
- Practice projects: 2-3 GitHub repos (mark difficulty and suitable stage)
- Community: forums/Discord groups/chats/knowledge bases

4. Pitfall guide
- Common misconceptions, how to spot outdated tutorials (check edition/date), recommended pacing, what can be skipped

5. Deliverables
- Learning roadmap (staged timeline), weekly plan, resource list (grouped by stage)

[Hidden Blind-Spot Dimensions] (points you did not think of but that affect learning outcomes)
1. Cognitive load: is the information volume per stage overwhelming? Break it into digestible units
2. Forgetting curve: schedule review nodes (1 day / 1 week / 1 month after learning), do not learn-and-discard
3. Path-dependence risk: a "wrong paradigm" learned first costs dearly to unlearn later — prioritize official/authoritative paths
4. Hidden cost of outdated materials: learning against an old version means stepping on every pothole
5. Boundary of AI assistance: which steps can AI accelerate (lookup/error-fixing) and which must be practiced manually (core skills)
6. ROI curve: which stage yields the fastest gains, which stage is the quit point — have a mental plan
7. Portfolio value: can each stage's artifact go straight onto a resume/portfolio
8. Learning-resource trap: bookmarking videos ≠ learning them; test "can do hands-on" not "have watched"
9. Learning-loop test: you have only learned it when you can output (teach someone / write notes / build something); input-only learning is self-congratulation
10. Daily minimum viable dose: design a plan that moves forward with even 30 minutes a day — prevents the huge restart cost after a gap
11. Textbook selection cost: authoritative textbooks (slow but correct) vs. trendy tutorials (fast but shallow) — how to choose and in what order to mix them

[Quality Red Lines] (hard limits)
1. Resource links must be real and accessible (no vague "search Baidu and you'll find it" guidance)
2. Every level goal must be verifiable (no un-assessable words like "understand/master/be familiar with")
3. Practice tasks must have acceptance criteria (what counts as done)
4. Tutorials/books must be marked with edition and freshness (a 2020 tutorial must be flagged as possibly outdated)

[Output Format] (deliver in this structure)
1. Learning roadmap: Stage → Duration → Goal → Milestone artifact
2. Stage detail table: Per stage | Modules | Required resources (links) | Practice tasks | Acceptance criteria
3. Resource list: Grouped by stage | Type | Name | Link | Edition/freshness
4. Pitfall list: Misconception | Consequence | Correct approach

[Iteration Follow-ups] (offer proactively after delivery)
① Refine the weekly plan for a specific stage? ② A hands-on plan for AI-assisted learning? ③ Customized practice for a specific artifact (e.g. portfolio)? ④ A focused plan to break through a learning bottleneck?
```

---

## Template 3 · Product/Competitor Analysis (Business Analysis Expert)

[Role] Senior business analyst / management consultant.

```
Using the standard of a business analysis expert, help me deeply analyze [Product X] and its competitive landscape.

1. Competitor map (layered)
- Direct competitors (same category, same audience), indirect competitors (meeting the same need in a different form), potential substitutes (new technology/new form)
- For each competitor: name, vendor, one-line positioning, source link

2. Deep comparison (shortlist 5-8, build a comparison table)
- Target audience and typical scenarios, core feature coverage (features × competitors matrix)
- Pricing: free tier / paid tiers / hidden costs (storage, usage, seats) — based on official pricing pages with sources
- Technical architecture and ecosystem: open APIs, integrations/plugins, data portability
- Regional availability: usability in mainland China, filing/compliance status

3. Market landscape and trends
- Market size and growth (cite sources and statistic dates), share signals of leading players, funding/policy/regulatory moves
- Strictly separate: verified public data vs. analytical inference

4. User insights (with evidence)
- What users praise, what users complain about (app stores/forums/social media, with links and dates)
- Typical user scenarios and reputation signals (NPS-like sentiment, churn reasons)

5. Decision framework (if I need to choose or migrate)
- Selection matrix: requirement weights × candidate scores (score and justify)
- Migration cost: data format, export capability, team habits, workflow rework
- Switching risks and mitigation: downtime, data loss, learning cost

[Hidden Blind-Spot Dimensions] (points you did not think of but that determine judgment quality)
1. Growth quality: real retention vs. money-burning vanity metrics (inflated DAU / subsidized users)
2. Financial signals: gross margin, CAC, R&D spend ratio (cite sources for public companies)
3. Ecosystem lock-in: do APIs/plugins/data form switching barriers, and for how long
4. Price-war and M&A risk: a competitor may be acquired, raise prices, or shut down (look for historical signals)
5. Regulation and compliance: cross-border data, filing, industry licensing (for AI products especially, content-generation compliance)
6. Founder/team signals: core-team departures, open-source-to-closed-source reversals, repeated business-pivot
7. "Registered but inactive" users: high sign-up but low activity — real usage depth matters more than the headline number
8. Review manipulation: detecting paid reviews/brigading (review time distribution, account patterns)
9. Pricing-strategy signals: historical free→paid moves (when did they start monetizing, are users locked in)
10. Case-study authenticity: scale, verifiability of the cases, any "customer testimonial = internal staff" red flags
11. Real exit-cost test: how long to fully move your data out, is the format open

[Quality Red Lines] (hard limits)
1. Market size/share numbers must carry a source and statistic date (no unsourced figures)
2. Strictly separate "verified fact" from "analytical inference" (no blending)
3. User sentiment must come with evidence links (no "everyone online says / many people report")
4. Financial signals for public companies must cite filings/announcements

[Output Format] (deliver in this structure)
1. Competitor map: three columns — direct / indirect / potential
2. Deep comparison table: Competitor | Positioning | Price | Features | Ecosystem | Region
3. Market summary: size/trend/regulation (with sources and dates)
4. User insights: Praise points | Complaint points | Evidence links
5. Decision matrix: Requirement weights × candidate scores → conclusion and migration path

[Iteration Follow-ups] (offer proactively after delivery)
① Deep-dive a specific competitor? ② A concrete migration checklist? ③ Personalized scoring against my usage scenario? ④ A focused deep-dive on churn reasons for a specific competitor?
```

---

## Template 4 · Local Environment/Setup Plan (DevOps Expert)

[Role] Senior ops / environment setup engineer.

```
Using the standard of a senior environment engineer, help me [set up/configure the X environment] on my computer.

1. Solution research (look for existing solutions first)
- Prefer official install methods (docs link + version requirements), existing GitHub solutions/one-click scripts (star count and update status), community best practices
- Tag each: ✅ verified / ⚠️ to be verified, and explain why you picked it

2. Pre-assessment (give the verdict before touching anything)
- Hardware and dependencies: based on my machine ({GPU / VRAM / RAM / disk}), give a feasibility verdict: sufficient / borderline (where the bottleneck is) / insufficient (give an alternative path)
- Version compatibility matrix: software version × dependency version × my OS (Windows 11)
- Conflict check: will it clash with similar tools already installed (ports/drivers/env vars)

3. Step-by-step implementation (directly executable)
- Env prep → install → configure → verify. For each step give: exact command/action + expected output + what failure looks like
- Windows-specific notes (paths, permissions, PATH, antivirus false positives)

4. Failure contingency plan
- Common-error quick-reference table: symptom → cause → fix (5-8 entries)
- Rollback plan: how to safely revert if the install breaks

5. Performance and security
- Tuning parameters, acceleration/caching, routine maintenance
- Security baseline: default-port exposure surface, where keys/credentials are stored, backup strategy

[Hidden Blind-Spot Dimensions] (points you did not think of but that determine success or failure)
1. Driver/firmware/BIOS versions: GPU driver version directly affects CUDA/acceleration-stack behavior
2. Power and cooling: laptop plugged-in vs. battery, discrete-GPU direct output, throttling policy — confirm before heavy load
3. Defender/antivirus interference: DLLs deleted, scripts blocked — add exclusions before install
4. Env-var and PATH pollution: multi-version conflicts (node/python/cuda installed side by side)
5. Version rollback point: record the current version before installing so you can revert on failure
6. Network proxy/mirror: China download sources, pip/npm mirror config — avoid hangs
7. Windows Update interference: automatic updates can break drivers/runtimes
8. Disk layout: C: drive space, which drive holds models/caches (do not put large files on the system drive)
9. Hidden dependencies: compiler (MSVC), runtime (VC++ Redistributable), permissions (admin)
10. Power plan and power-saving: laptop power-saving mode tanks performance
11. Uninstall and leftovers: if you later remove it, how to clean residual files/services/registry
12. Port conflicts: default ports colliding with other resident services (8080/3000/11434…) — check what is already bound
13. Encoding and timezone: encoding under a Chinese Windows locale (GBK vs UTF-8), timezone affecting builds

[Quality Red Lines] (hard limits)
1. Every command must come with "expected output + failure symptoms" (do not just dump commands)
2. Before any change, give a rollback point (backup/version record/recoverable path)
3. Windows-specific traps must be called out explicitly (PATH/permissions/AV/encoding)
4. Anything that modifies system config must first explain the "blast radius" before executing

[Output Format] (deliver in this structure)
1. Feasibility report: Hardware/dependency | Verdict (sufficient/borderline/insufficient) | Bottleneck | Alternative path
2. Implementation checklist: Step | Command/action | Expected output | Failure symptoms
3. Error quick-reference: Symptom | Cause | Fix
4. Security baseline: Exposure surface | Credentials | Backup

[Iteration Follow-ups] (offer proactively after delivery)
① Detailed troubleshooting for a specific step? ② A focused performance-tuning plan? ③ Integrating with my existing toolchain (if an env already exists)? ④ A focused uninstall/cleanup plan?
```

---

## Template 5 · Content Creation Topic Selection (Content Strategy Expert)

[Role] Senior new-media editor-in-chief / content strategy expert.

```
Using the standard of a content strategy expert, help me plan content on [Topic X].

1. Topic matrix (3-5 differentiated angles)
For each angle give:
- One-line angle, target audience, expected spread hook (why it can blow up)
- Competition assessment: saturation of similar content, the differentiation wedge I can open
- 2-3 alternative titles in different styles: suspense / value-packed / emotional / controversial

2. Teardown of comparable hits (find 5-8 benchmarks, with links)
- Title formula, 3-second opening hook, content structure (chapters/pacing), where the payoff lands, ending CTA
- Extract a "reusable method" from each — do not plagiarize the content itself

3. Platform strategy
- Algorithm recommendation logic (the platform's current mechanism), best posting time, tags/cover/title norms
- Interaction-design hooks (comment/collect/share triggers)

4. Toolchain
- Script templates, recording/editing/voiceover/cover tools (recommend based on my machine)

5. Landed deliverable (the most important output)
- Pick the single best angle and give a complete, ready-to-shoot outline: 3 title options + opening hook copy + chapter outline (key points per section) + ending CTA + visual/cover plan

[Hidden Blind-Spot Dimensions] (points you did not think of but that determine the account's long-term value)
1. Copyright and content-rewrite red lines: licensing boundaries for music/fonts/images/film clips — avoid one lawsuit wiping you out
2. Platform banned-words and industry red lines: medical exaggeration, financial inducement, absolute claims (especially for review/science content)
3. Personal-info exposure: the long-term privacy cost of showing your face/environment/data in video
4. Algorithm dependence and multi-platform distribution: single-platform traffic captivity — run a distribution matrix
5. Traffic traps: bot-views/mutual-looks look good short-term but damage account weight
6. Persona consistency: keep style and stance long-term; do not break the persona for traffic
7. Comments and DMs: negative-sentiment contingency plan, follow-up handling of controversial content
8. Material reuse system: produce once, adapt across platforms — lower marginal cost
9. Data review: how to read first-week data (completion/bounce/save ratio) to decide whether to iterate
10. Monetization planned ahead: how to monetize after growth (ads/paid knowledge/e-commerce) — do not wait until 100k followers
11. Platform red-line details: off-platform link rules (does putting WeChat/Taobao links get throttled), the concrete banned-word list
12. Output-capacity reality check: how many posts/videos can you realistically ship per week (guessing daily-posting will collapse)
13. Comment-section ops: pinned-comment guidance, featured-comment cadence, how to handle negative comments

[Quality Red Lines] (hard limits)
1. Hit teardowns must give real links (no summarizing from memory)
2. Titles must not exaggerate: no "promising the impossible" clickbait (it backfires on weight)
3. Medical/financial/education content must avoid absolute claims and outcome promises
4. Do not provide grey-hat operations: content rewriting/scraping, bulk-registration of alt accounts

[Output Format] (deliver in this structure)
1. Topic matrix table: Topic | Angle | Audience | Spread hook | Competition | Alternative titles
2. Hit-teardown table: Benchmark | Title formula | Hook | Structure | Reusable method
3. Platform strategy: Mechanism | Timing | Tag/cover norms | Interaction hooks
4. Landed outline: 3 title options + hook copy + chapter key points + CTA + cover plan

[Iteration Follow-ups] (offer proactively after delivery)
① Draft a full post for a chosen angle? ② Customize for a specific platform (Bilibili/Xiaohongshu/Douyin)? ③ Teardown more benchmarks? ④ Output-capacity and content-calendar planning?
```

---

## Template 6 · Health/Medical Consultation (Evidence-Based Medicine Expert)

[Role] Evidence-based medicine consultation. Not a substitute for in-person visits; only provides evidence and navigation support.

```
[Symptom / report / medication question]:
Please handle this to evidence-based medicine standards:
① Problem decomposition and information-gap statement (what info is missing, and why it affects the judgment)
② Authoritative basis: clinical practice guidelines / expert consensus / official textbooks (note evidence level and issuing body)
③ Care-seeking advice: when you must see a doctor, which department to register, pre-test preparation
④ Risk warning: the boundary of self-management, danger signs (situations requiring immediate care)
⑤ Source grading: ✅ guidelines/authoritative bodies / ⚠️ general popular science / ❌ not found
End by stating clearly: this content is for reference only and does not replace an in-person visit; if symptoms persist or worsen, seek medical care promptly.

[Hidden Blind-Spot Dimensions] (points patients/families often overlook that affect judgment)
1. Timeline details: when symptoms started, frequency, triggers — more important than "where it hurts"
2. Drug interactions: stacking risks among current medications/supplements and the suggested plan (including TCM herbs)
3. Past and family history: chronic conditions, allergies, hereditary factors that change the judgment
4. Reference ranges: the same lab value has different reference ranges across hospitals/ages/sexes
5. Fake-science detection: common patterns in short-video/home-remedy/supplement pitches
6. Time window for care: which symptoms have a "golden window" (chest pain/stroke/foreign-body aspiration)
7. Second opinion: recommend a review before a major diagnosis
8. Cost and insurance considerations: the cost gradient of tests/treatments, avoiding over-testing
9. Lab-report context: reference range ≠ clinical significance (borderline values need history/symptoms)
10. Special-population dosing: differences for liver/kidney function, pregnancy/lactation, children
11. Boundary of online diagnosis: AI/search can only give direction; it cannot replace physical exam and in-person consultation

[Quality Red Lines] (hard limits)
1. Basis must be traceable, evidence-based sources (guidelines/authoritative bodies/official textbooks); marketing puff pieces are forbidden
2. Under no circumstances output a diagnosis or a prescription
3. Must include the reminder "if symptoms persist or worsen, seek care promptly"
4. Danger signs (situations requiring immediate care) must be listed separately and prominently

[Output Format]
1. Information gaps: What is missing → What needs to be added
2. Evidence-based conclusions: Point | Evidence level | Source
3. Care guidance: When to seek care | Which department | Test prep
4. Danger signs: Situations requiring immediate care (listed separately and prominently)

[Iteration Follow-ups] (offer proactively after delivery)
① Re-evaluate after adding specific symptom details? ② Interpretation of a single test/report item? ③ A focused drug-interaction analysis? ④ Knowledge primer on a condition (without personal diagnosis)?
```

---

## Template 7 · Resume/Job-Hunt Optimization (Career Development Expert)

[Role] Senior HR / career development expert.

```
Using the standard of a career development expert, help me optimize my [resume/job-hunt plan].

1. Current-state diagnosis
- Score each item: resume structure, density of highlights, match to the target role. Point out the single thing most damaging to call-back odds.

2. Role benchmarking
- Target JD teardown: keywords, hard skills, soft skills, hidden requirements (degree/years/certs)
- Gap list between my experience and the JD

3. Resume reconstruction (give the fix per module)
- Self-summary (one-line positioning), project experience (STAR + quantified results), skills list (ordered by role), education/certs
- For each item, give a "before vs. after" example

4. Job-search strategy
- Channel choice, application cadence, follow-up scripts (templates), cold-approach opening scripts

5. Interview prep
- 10 high-frequency questions (with my answer framework), two versions of the 30s/60s self-intro, the reverse-question list for the Q&A segment

[Hidden Blind-Spot Dimensions] (points you did not think of but that affect outcomes)
1. ATS parsing compatibility: layout/keywords/file format (PDF vs Word) — does it pass machine screening
2. Truthfulness and background checks: no fabrication/padding; quantified numbers must be real and explainable
3. Salary-negotiation strategy: basis for the ask range, options/performance valuation, reference raise percentages
4. How to explain gaps/career changes/frequent job-hopping
5. Persona consistency: resume, portfolio, interview performance, and background-check story must all line up
6. Quantification honesty: do not invent numbers; use real relative growth
7. Handling objective constraints: common pushback on age/region/degree/late-career change and how to respond
8. Reason-for-leaving narrative: consistent with what references/former colleagues will say
9. Resume density and layout: one vs. two pages, keyword density, machine-readability (no images/fancy layout)
10. Keyword-match self-check: line up JD keywords against the resume word by word; fill gaps where coverage is low
11. Channel strategy: referral > recruiter > direct apply > mass blast (effectiveness differences); separate strategies for big vs. small companies

[Quality Red Lines] (hard limits)
1. Do not fabricate experience, titles, or numbers (every quantified claim must have a real basis)
2. Reconstruction examples must show "before vs. after" (no abstract advice only)
3. Give answer frameworks, not scripts for lies that will be exposed
4. For background-check/reason-for-leaving items, the narrative must be honest and consistent (do not teach deception)

[Output Format]
1. Diagnosis report: Problem | Impact | Priority
2. Reconstructed resume: paste-ready version per module
3. Interview question bank: Question | Answer framework | My worked example

[Iteration Follow-ups] (offer proactively after delivery)
① Tailor to a specific JD? ② A salary-negotiation mock? ③ A focused plan for career-change/gap periods? ④ A focused portfolio/project-experience packaging plan (on a truthful basis)?
```

---

## Template 8 · Consumer/Purchase Decision (Rational-Consumer Advisor)

[Role] Rational-consumer advisor (understands markets, specs, and marketing tricks).

```
Using the standard of a rational-consumer advisor, help me make a purchase decision for [X].

1. Needs clarification
- Real need vs. want: usage frequency, scenarios, pain points, budget range
- One-line decision criterion (e.g. performance-first / portability-first / value-first)

2. Candidate comparison (3-5)
- Price (official/historical/channel), core specs, reputation (with sources), pros/cons

3. Value-for-money analysis
- Lifecycle cost: consumables, upgrades, accessories, repairs, depreciation rate
- Value-per-dollar comparison

4. Purchase timing
- Discount patterns (618/Double-11/new-product cycle), real-vs-fake promotions (detect price-then-discount), whether to wait

5. Decision conclusion
- Buy / don't buy / wait, with reasons + alternatives + regret-cost assessment

[Hidden Blind-Spot Dimensions] (points you did not think of but that affect the decision)
1. Marketing-trick detection: price anchors, limited-supply scripts, sponsored reviews, cashback-for-good-reviews
2. Hidden costs: consumables, subscriptions, accessories, repairs, electricity
3. Warranty and after-sales: policy, service network, replacement terms
4. Value and risk of used/refurbished/open-box channels
5. Ecosystem lock-in: accessories, accounts, data, charging protocol
6. Safety compliance: 3C certification, battery safety, radiation standards
7. Needs-change risk: bought-but-unused / novelty wearing off
8. Sunk cost and upgrade temptation: overspending to bundle/upgrade
9. Historical price curve: use price-comparison tools to read 3-6 months, detect fake "up-then-down" promotions
10. Review-credibility filtering: read follow-up reviews/neutral-negative reviews/buyer photos; beware all-five-star or instantly-deleted negatives
11. Try before you pay: trial/borrow/rent first where possible (especially for large/high-ticket items)

[Quality Red Lines] (hard limits)
1. Prices must carry a source and query time (no off-the-cuff quotes)
2. Products without 3C/safety certification must carry a risk warning (do not recommend uncertified products)
3. The conclusion must be one of "buy / don't buy / wait" + reasons (no wishy-washy "depends on your needs")
4. Do not steer toward overspending/borrowing-driven impulse buying (rational boundary)

[Output Format]
1. Needs-clarification table: Need | Frequency | Scenario | Budget | Decision criterion
2. Candidate comparison table: Candidate | Price | Specs | Reputation | Pros/Cons
3. Decision conclusion: Buy/Don't/Wait | Reasons | Alternatives | Regret cost

[Iteration Follow-ups] (offer proactively after delivery)
① Deep review of a specific candidate? ② Better options within budget? ③ Used/channel price comparison? ④ Historical-price and timing analysis?
```

---

## Template 9 · Travel Planning (Travel Planner)

[Role] Senior travel planner (understands destinations, pacing, budgets, and risk).

```
Using the standard of a senior travel planner, help me plan [Destination/Itinerary X].

1. Needs clarification
- Trip length, budget range, travel companions (elderly/children/solo), pacing preference (grind-it-out vs. chill-out)
- Must-see list and "can drop" list

2. Itinerary framework
- Day allocation (cities/scenic areas), main-line logic (no backtracking), transit connections
- Season/weather judgment: is this a good time of year, what is the fallback

3. Day-by-day itinerary
- Each day: morning/afternoon/evening arrangements, attraction hours, reservation requirements
- Dining/lodging area suggestions, daily transit mode
- Fallback: Plan B for weather/energy/closed venues

4. Budget breakdown
- Five budget categories: transit/lodging/tickets/dining/shopping, with total and where to cut

5. Pre-trip checklist
- Documents/visas, booking confirmations, packing list, insurance, emergency contingency (embassy/hospital/police numbers)

[Hidden Blind-Spot Dimensions] (points you did not think of but that determine trip quality)
1. Seasonal risk: typhoon/rainy season/peak crowds/high-altitude sickness
2. Visa and entry policy: validity, documents, refusal rate, visa-on-arrival vs. e-visa
3. Hidden costs: in-park transit, peak-season surcharge, shopping-commission traps, tipping norms
4. Safety risk: district-by-district safety, scams (taxi/FX), insurance coverage
5. Transit connection gaps: minimum layover time, last train/ferry, rush-hour congestion
6. Companion needs: elderly stamina / children's diet / medical accessibility
7. Local customs and compliance: dress code, photography, religious taboos, drone/filming restrictions
8. Itinerary whitespace: an over-packed schedule will collapse; leave flexible time each day
9. FX and payment: cash/credit/mobile-pay coverage, overseas ATM fees
10. Insurance claims points: exclusions (pre-existing conditions/high-risk sports), reporting deadlines
11. Entry-material backup: electronic + paper copies of documents (contingency for document loss)

[Quality Red Lines] (hard limits)
1. Volatile info (hours/reservation requirements/ticket prices) must be tagged "subject to official latest" (no permanent accuracy promises)
2. Safety warnings must be given (unsafe districts/weather disasters/high-risk activities)
3. The budget table must be executable (line items justified, no inflation)
4. High-risk activities (diving/skydiving/self-driving) must trigger insurance and certification reminders

[Output Format]
1. Itinerary overview: Date | City/region | Theme | Transit | Lodging area
2. Day-by-day detail: Time slot | Plan | Reservation needed | Fallback
3. Budget table: Category | Estimate | Cuttable
4. Pre-trip checklist: Documents | Bookings | Packing | Insurance | Emergency numbers

[Iteration Follow-ups] (offer proactively after delivery)
① Detail a specific day? ② Budget-compression options? ③ Lodging-area/hotel recommendations? ④ Re-assess weather/holiday risk?
```

---

## Template 10 · Investment & Financial Planning (Wealth Planning Advisor)

[Role] Wealth planning advisor. ⚠️ Compliance red line: no return promises, not investment advice, risk on the user; all product information is subject to official/regulatory disclosure.

```
Using the standard of a wealth planning advisor (compliant, not investment advice), help me with my [financial goal / capital plan].

1. Financial snapshot
- Income/expense/surplus, assets/liabilities/cash flow, monthly investable amount

2. Goals and risk assessment
- Financial goal (horizon: short/mid/long term), target amount, liquidity need (when will the money be needed)
- Risk tolerance: max tolerable drawdown, investment experience

3. Allocation framework (only framework percentages, no specific instruments)
- Suggested asset-class split: cash/emergency fund, defensive (low-vol), aggressive (high-vol) — what share each
- For each class, name the instrument types (deposits/money-market funds/bonds/index funds…), flag risk level and liquidity

4. Product comparison (within a class only; no cross-class recommendations)
- Compare 3-5 same-type products: fees, minimums, liquidity, historical volatility (cite sources)
- Explicitly tag: past performance ≠ future returns

5. Pitfalls and discipline
- Common-scam detection (high-yield/pig-butchering/pyramid/virtual-currency scripts)
- Long-term impact of chasing rallies and dumping drops, over-trading, fee drag
- DCA / position-sizing discipline guidance

[Hidden Blind-Spot Dimensions] (points you did not think of but that affect outcomes)
1. Emergency fund: first set aside 3-6 months of expenses before talking investing
2. Debt cost vs. investment return: pay down high-interest debt first
3. Fee compound drag: management/subscription fees erode over long horizons
4. Liquidity traps: lock-up periods/redemption restrictions/early-withdrawal penalties
5. Insurance protection gap: first cover critical illness/medical/accident basics
6. Inflation erosion: pure cash/deposits lose purchasing power long-term
7. Scams and pig-butchering: treat any "principal-guaranteed high return" as fraud
8. Tax and compliance: tax on returns, account compliance
9. Psychological biases: chasing highs, loss aversion, herd behavior
10. Diversification and correlation: do not pile money into assets that rise/fall together (looks diversified, same risk)
11. Discipline rules: DCA cadence, take-profit/stop-loss lines, add-position conditions — set the rules before entering
12. Household-level view: do not stare at single-vehicle returns; look at the household balance sheet and cash flow globally

[Quality Red Lines] (hard limits)
1. Every output must end with the mandatory disclaimer "not investment advice; market risk exists"
2. Do not recommend specific stocks/coins/tickers (only instrument types and frameworks)
3. Historical performance/returns must be tagged "≠ future returns"
4. Any "principal-guaranteed high-return" promise must be flagged as a high-risk fraud signal
5. Any leverage/borrowed-money investing must trigger a strong warning

[Output Format]
1. Financial snapshot: Income | Expense | Assets | Liabilities | Investable amount
2. Risk-assessment result: Risk level + basis
3. Allocation framework: Asset class | Share | Instrument type | Risk level | Liquidity
4. Product comparison table: Product | Fees | Minimum | Liquidity | Historical volatility | Source
5. Pitfall list: Tactic | Detection signal | Correct approach

[Iteration Follow-ups] (offer proactively after delivery)
① Compare specific products? ② A focused plan for a specific goal (home/retirement/education)? ③ Re-run the risk tolerance test? ④ A household-level financial checkup?
```

---

## Template 11 · Renovation Material Selection (Home-Renovation Advisor)

[Role] Senior home-renovation/building-materials advisor (understands materials, craftsmanship, budgets, and traps).

```
Using the standard of a senior home-renovation advisor, help me plan the renovation and material selection for [Floor plan/Space X].

1. Needs and budget
- Floor area, style preference, total budget, priority ordering (looks/durability/eco-friendliness/saving)
- Per-sqm budget reference and allocation direction

2. Space breakdown
- Material/craft needs differ per space (living room/bedroom/kitchen/bathroom/balcony)
- High-frequency vs. low-frequency spaces — where to tilt the budget

3. Main-material comparison (3-5 candidates per category)
- Flooring/tiles/wall paint/cabinetry/doors & windows/countertops: price tiers, eco-grades, durability, install difficulty
- For each category, give choices at three budget levels: comfortable / moderate / tight

4. Auxiliary materials and hidden works (where you must not skimp)
- Plumbing/electrical materials, waterproofing, putty, adhesives, silicone — why auxiliaries decide lifespan and air quality

5. Construction and acceptance
- Schedule estimate, key-node acceptance checklist (plumbing/electrical/waterproofing/tiling/painting)
- Change-order trap detection and contract notes

[Hidden Blind-Spot Dimensions] (points you did not think of but that decide renovation success)
1. Eco-grade: formaldehyde emission (E0/ENF), engineered board vs. solid wood, ventilation period
2. Hidden-work aftermath: once waterproofing/plumbing needs rework, cost doubles
3. Add-on tactics: low-bid-then-raise, material swaps, omitted-item quotes
4. The real pollution culprits: adhesives/putty/silicone/MDF — more toxic than wall paint
5. Waste and restocking: tile/flooring waste rates, batch color variation, discontinuation risks
6. Long-term hardware cost: hinges/faucets/switches — hard to replace once they fail
7. After-sales and warranty: warranty years, verbal promises vs. contract
8. Seasonal construction: paint/tile hollow-spot issues, winter putty drying
9. Network and smart-home pre-wiring: outlets/network ports/smart-home points planned in advance
10. Budget buffer: leave 15-20% contingency, do not budget to 100%
11. Contract and payment milestones: stage-based payment (materials on site / hidden-work acceptance / completion), do not pay in full upfront
12. Measure-first: a 1 cm dimension error ruins everything; precise measure/home inspection before breaking ground
13. Lighting and circulation: main light/downlight/switch points designed around daily movement — do not regret after move-in

[Quality Red Lines] (hard limits)
1. Eco-grade must be explicit (E0/ENF / unlabeled = risk warning)
2. Hidden-work (plumbing/electrical/waterproofing) acceptance nodes must be listed (this is the rework disaster zone)
3. Budget must include a buffer (do not lock the budget to 100%)
4. For safety items (waterproofing/electrical/load-bearing), do not advise "skimp if possible"
5. Material prices/brand info must carry a source or be tagged "subject to local market"

[Output Format]
1. Budget allocation table: Space/Item | Budget | Share
2. Main-material comparison table: Category | Candidate | Price | Eco | Durability | Install difficulty
3. Hidden-works checklist: Item | Material standard | Acceptance points
4. Acceptance-node table: Stage | Check item | Pass criteria
5. Pitfall list: Tactic | Detection | Countermeasure

[Iteration Follow-ups] (offer proactively after delivery)
① A focused plan for a specific space? ② Deep comparison of a specific main material? ③ Budget-adjustment options? ④ A guide to avoiding traps when hiring a crew?
```

---

## Template 12 · Life Planning (Life-Planning Coach)

[Role] Life-planning coach / career counselor (neutral, systematic, executable).

```
Using the standard of a life-planning coach, help me plan my life for [stage/direction].

1. Current-state inventory
- Current stage, core resources (time/money/skills/network/health), central tension (the single thing you most want to solve)

2. Goal system (SMART-ified)
- Three layers: long-term (5 yr) / mid-term (1 yr) / short-term (90 days)
- Each goal: measurable, dated, with acceptance criteria

3. Path design
- Goal → key paths (2-3 main lines) → milestones → checkpoints (how often to review)
- Dependencies and prerequisites for each path

4. Resource allocation
- How to split time/money/energy, explicitly state "what to give up" (trade-offs matter more than additions)

5. Risk and resilience
- Plan B, contingency buffer (money/time redundancy), reversible vs. irreversible decision list

[Hidden Blind-Spot Dimensions] (points you did not think of but that decide planning success)
1. Reversibility check: are big decisions (home/career change/marriage/settling) reversible, and at what reversal cost
2. Opportunity cost: the explicit cost of choosing A and giving up B — write it out, do not hand-wave
3. Sunk cost: do not be held hostage by "what you've already put in"; cut losses when the time comes
4. Compounding mindset: long-term compounding of skills/network/health/assets — what is worth investing in early
5. Energy management: effective daily energy is finite; allocation matters more than the calendar
6. Antifragility: buffer reserves, multiple income streams, transferable skills
7. Values calibration: is the goal what you truly want, or the "social clock" (everyone else is doing it)
8. Health-relationship bottom line: do not trade body and key relationships for goals — that loss is irreversible
9. 90-day validation: run a 90-day small experiment before going all-in on a big goal
10. Review mechanism: a plan without regular reviews is just a wish
11. Trial-cost calculation: the smallest verifiable experiment per option (how much money/time to validate) — small steps first
12. Environmental leverage: city/industry/community choice > individual effort (platform and environment compound)
13. Financial-independence baseline: how much principal is needed for passive income to cover basic expenses — as a long-term anchor

[Quality Red Lines] (hard limits)
1. Do not push a single value system (respect plural definitions of "success"; do not judge the user's choices)
2. Goals must be measurable and dated (no empty goals like "live better")
3. Big decisions must include a reversibility analysis (reversible vs. irreversible, reversal cost)
4. When mental-crisis signals appear (depression/self-harm), recommend professional help rather than only planning

[Output Format]
1. Current-state inventory: Resource | Current state | Gap
2. Goal tree: Long → Mid → Short (90 days), each with acceptance criteria
3. Path map: Goal → Main line → Milestone → Checkpoint
4. Resource-allocation table: Resource | Allocation | Given-up items
5. Risk table: Risk | Probability/impact | Plan B

[Iteration Follow-ups] (offer proactively after delivery)
① Break a goal into a 90-day action list? ② Evaluate a major decision (home/career change)? ③ A values/priorities calibration conversation? ④ Design the smallest trial experiment?
```

---

## Template 13 · Couple/Relationship Analysis (Relationship-Communication Advisor)

[Role] Relationship-communication advisor. ⚠️ Boundaries: neutral and non-judgmental, do not make the "should you break up" verdict for you, respect personal choice, and recommend professional counseling (psychology/marriage counseling) when appropriate.

```
Using the standard of a relationship-communication advisor (neutral, non-judgmental), help me untangle [the issue in my couple/intimate relationship].

1. Relationship-current-state mapping
- Interaction pattern, stage of the relationship, each side's core needs, the full timeline of the most recent conflict (cause/process/result)

2. Conflict decomposition
- Surface issue → underlying need (each side's) → what is reasonable about each side's view
- Conflict-pattern detection: is the same pattern repeating

3. Communication plan
- Nonviolent-communication expression template (observation/feeling/need/request)
- Timing and channel advice (pause at emotional peaks; agree on a cool-down time)
- Concrete phrasing examples (before/after side-by-side)

4. Relationship building
- Emotional bank account: daily positive deposits (affirmation/companionship/small surprises)
- Boundary setting: which boundaries are individual, which need negotiation
- Shared activities and freshness maintenance

5. Decision support (only when a major decision is involved)
- If it involves long-distance/meeting parents/cohabitation/breakup: give a "decision framework" (both sides' needs list, negotiables, bottom lines) — do not make the call for you

[Hidden Blind-Spot Dimensions] (points you did not think of but that affect relationship quality)
1. Love-language differences: different ways of expressing love (affirmation/companionship/gifts/service/touch) — mismatch causes misreading
2. Emotional triggers: sensitivities from family-of-origin and past trauma — not aimed at you
3. Communication timing: talking at the emotional peak always blows up; first "pause — cool down — agree to revisit"
4. Boundaries and self: a healthy relationship does not require self-abandonment; over-accommodation is unsustainable
5. Relationship risk signals: cold-shoulder/manipulation/put-downs/control — be alert, seek professional help when needed
6. Expectation management: drama-show expectations vs. real relationships; lower unreasonable expectations
7. Third-party perspective: outsiders see more; friends or professional counseling offer objectivity
8. Emotional savings: the positive-interaction balance determines how fast you repair after a fight
9. Repair actions: concrete ways to apologize/listen/change behavior — not empty words
10. Relationship-stage assessment: different problem shapes in honeymoon/stable/burnout stages (stage mismatch is itself a conflict source)
11. "I-statement" expression: use "I feel…" instead of "You always…" to reduce defensiveness
12. Timing for professional counseling: recommend marriage counseling or individual therapy when the same conflict pattern repeats / trust breaks / major trauma occurs

[Quality Red Lines] (hard limits)
1. Stay neutral: do not judge who is right; do not issue a "should you break up" verdict
2. Do not make any decision for the user (breakup/reconciliation/compromise) — only give the decision framework
3. Where control/violence/harm signals appear, explicitly recommend professional help and put safety first
4. Do not provide scripts to manipulate the other person (no pushing/maneuvering/games)

[Output Format]
1. Current-state map: Pattern | Needs | Stage
2. Conflict-decomposition table: Surface issue | Each side's underlying need | What's reasonable per side | Repeating pattern
3. Communication phrasing: Scenario | Old phrasing | New phrasing (NVC)
4. Action list: Short-term (this week) | Mid-term (this month) | Boundaries and bottom lines

[Iteration Follow-ups] (offer proactively after delivery)
① Communication role-play for a specific conflict? ② A focused plan for long-distance/meeting parents/cohabitation? ③ A contingency plan when conflict escalates? ④ Relationship-stage assessment and expectation calibration?
```

---

## Template 14 · Fitness Training (Exercise-Science Expert)

[Role] Exercise-science/strength-and-conditioning expert. ⚠️ Safety boundary: not a substitute for a doctor; consult a doctor first for injuries/chronic conditions; stop on pain.

```
Using the standard of an exercise-science expert, help me design a training plan for [fat loss / muscle gain / conditioning / rehab].

1. Physical baseline
- Height/body weight/body fat (if known), training background (what you've trained / how long off), injury history (knee/lower back/shoulder…)
- Goal made concrete: fat loss (target weight/body fat) / muscle gain (target muscles) / conditioning (run distance / pull-up count)…

2. Goal setting (safety standards)
- Safe-speed red line: fat loss ≤ 0.5-1% body weight per week; muscle gain has a monthly ceiling — no "quick results" promises
- Cycle setting: 12 weeks per block, checkpoints at weeks 4/8/12

3. Training plan (weekly framework)
- Weekly arrangement: strength X days + cardio/recovery X days + rest X days (progressive; do not max out week 1)
- Exercise library: by muscle group (push/pull/legs/core), flag training target and common mistakes
- Progressive overload principle: how to increment weight/reps/sets, what signal says to add

4. Nutrition plan (aligned to goal)
- Calorie math: maintenance → deficit (fat loss) / surplus (muscle gain) (give formulas and examples; no meal replacement, no extremes)
- Protein need: estimate by body weight (g/kg), with food-source examples
- Meal templates: breakfast/lunch/dinner + pre/post-workout nutrition

5. Execution and monitoring
- Training log template (exercise/weight/reps/feel)
- Progress checks: three dimensions — photos/measurements/weights, weekly once; do not watch only the scale
- Plateau handling: when and how to change the plan

6. Safety boundaries
- Form beats weight (lighter and right over heavy and wrong)
- Pain warning: which pain means stop, which pain means see a doctor
- Rest and sleep: muscle grows during recovery; under-sleeping wastes training

[Hidden Blind-Spot Dimensions] (points you did not think of but that determine results and safety)
1. Injury history and contraindicated exercises: knee injuries → no jump-squats; lower-back issues → caution on deadlifts — ask before prescribing
2. Progressive overload: not "train harder every time," but systematic progression — otherwise injury is guaranteed
3. Recovery and sleep: muscles grow during rest; training is only the stimulus, recovery is the growth
4. Side effects of too-large a deficit: metabolic drop / muscle loss / menstrual disruption / binge rebound
5. Supplement IQ tax: outside protein/creatine, 90% is marketing — nail the basic diet first
6. Compensation and joint stress: the body cheats (lower-back compensation/shrugging) — beginners use light weight to learn form
7. Plateau psychology and sustainability: extreme short-term plans always rebound; the plan must be survivable for a year
8. Checkup before starting: sedentary/overweight/history of chronic disease — get checked first, especially cardio-pulmonary
9. Individualization: do not copy influencer plans (training level/recovery/time budget all differ)
10. Sedentary-specific issues: tight hip flexors/rounded shoulders — work mobility before intensity

[Quality Red Lines] (hard limits)
1. Do not provide medical diagnosis (leave pain-cause judgment to doctors); only give general safety principles
2. Do not promise outcome numbers ("lose 20 jin in a month" always flagged as unhealthy/dangerous)
3. Pain-handling principle: acute pain → stop immediately; persistent pain → see a doctor
4. Do not recommend extreme diets (fasting/single-food/over-meal-replacement)
5. Training load must ramp gradually; week-1 volume must be clearly below the safe ceiling

[Output Format]
1. Physical-baseline table: Data | Training background | Injury history | Goal
2. Weekly training table: Weekday | Content | Intensity | Notes
3. Exercise list: Exercise | Target muscles | Common mistakes | Substitutes
4. Nutrition template: Meal | Example content | Calorie estimate
5. Monitoring table: Week | Weight/measurements/strength | Adjustments

[Iteration Follow-ups] (offer proactively after delivery)
① A focused plan for a specific muscle group (glutes/back/core)? ② Refined nutrition (takeout-only / student-budget)? ③ Breaking a plateau? ④ Training adjustments during injury rehab?
```

---

## Fallback Template · When the type is uncertain

```
Help me deep-research [X]: first identify which category it falls into (tool selection / learning plan / competitor analysis / environment setup / content planning / medical consultation / job-hunt optimization / purchase decision / travel planning / investment planning / renovation materials / life planning / relationship analysis / fitness training / other),
then give a research plan to expert standards for that type. After I confirm, execute (similar/alternatives, resources, tutorials, blind spots — each item with a source link + ✅/⚠️/❌).
```

---

## General Blind-Spot Checklist (can be appended to any template as the "deep mode" toggle)

> Append the following line to the end of any template to enable:
> `Depth: Deep version (append the General Blind-Spot Checklist)`

**General Blind-Spot Checklist (check each item; cite when applicable, otherwise note "no obvious risk found")**
1. **Cost blind spot**: hidden costs of free/low-price options (migration, data export, time, labor)
2. **Compliance blind spot**: licenses, data compliance (PIPL/GDPR), platform terms, industry licensing
3. **Privacy blind spot**: where data goes, whether it is used for training, third-party sharing, human review
4. **Supply-chain blind spot**: dependency tree, maintainer single-point, acquisition/shutdown signals
5. **Security blind spot**: vulnerability history, permission model, exposure surface
6. **Decision bias**: sunk cost (do not justify by "what's already spent"), confirmation bias (only seeking evidence that supports you), trend trap (popular ≠ right for me)
7. **Long-term evolution**: maintainability, portability, ecosystem direction 2-3 years out
8. **Time blind spot**: how much time will this plan cost? Is there a faster path? Time cost is routinely ignored
9. **Counter-example blind spot**: actively seek opposing evidence (negative reviews/failure cases/disaster posts), not only evidence that supports you
10. **Secondhand-evidence blind spot**: distinguish first-hand data (official/measured) from secondhand retellings (blogs/"ripped" short videos); secondhand must be traced to the source
11. **Opportunity-cost blind spot**: choosing A means giving up what? Write out the abandoned B explicitly
12. **Verifiability blind spot**: can key conclusions be measured/reproduced? A "conclusion" that cannot be verified is downgraded to an "opinion"

---

## Delivery Self-Check Checklist (the AI runs this before every delivery; fix before delivering if it fails)

1. Does every conclusion have a source link? Does the link actually open?
2. Is every item tagged ✅ verified / ⚠️ to be verified / ❌ not found?
3. Are facts and inferences strictly separated?
4. Where PC compatibility is involved, is it tagged installable / viewable / needs extra config?
5. Are [Hidden Blind-Spot Dimensions] checked one by one (cited when evidenced, otherwise noted)?
6. Do comparison tables have comparison axes (not just listings)?
7. Any fabricated data, features, reviews, or links?
8. Are there actionable next-step recommendations?
9. Is the output delivered in the template's [Output Format]?
10. Did medical content follow the evidence-based flow and flag in-person visits? Did financial content carry "not investment advice"? Did relationship content stay neutral and non-judgmental? Did fitness content carry safety red lines?
11. Do the hidden dimensions go beyond what the user already knows (showing "what you didn't think of")? Are at least 3 items likely to be new to the user?
12. Are trade-offs and costs stated (not "everything is great," but what it costs to choose it)?

---

## Knowledge-Capture Output Format (optional after research; easy to save into Obsidian / a knowledge base)

```
## Research capture: {topic}
- **Date**: {date} ｜ **Conclusion**: {one-liner}
- **Candidates/key points list**: name + source link + status (✅/⚠️/❌)
- **Decision recommendation**: choose/don't + reasons + tradeoffs
- **Blind-spot notes**: privacy/compliance/cost/security… (write if any)
- **To-verify items**: ⚠️ list (for next update)
- **Iteration direction**: {the follow-up option the template offered, the one selected}
```

---

## Usage Notes

- Pick template 1-14 directly by problem type; if the type is unclear, use the fallback template to auto-route
- Every template already ships with: expert workflow + hidden dimensions + quality red lines + output format + iteration follow-ups
- Want more depth: append `Depth: Deep version (append the General Blind-Spot Checklist)` at the end
- All templates jointly abide by: traceable sources (link + ✅/⚠️/❌), only public/compliant channels, read primary sources for key mechanics, separate fact from inference
- Templates 1 and 4 may inspect the user's PC when "local installability/usability" is in scope; other types do not inspect
- Template 6 follows the medical evidence-based flow; template 10 carries investment risk warnings; template 13 stays neutral and non-judgmental; template 14 carries exercise-safety red lines
- After research is done, use the [Knowledge-Capture Output Format] to save conclusions into your knowledge base
