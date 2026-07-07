# Scratchpad

> The raw workbench. Everything lands here first — unfiltered thoughts, conversation notes, half-formed hypotheses, reading trails, contradictions. Nothing here is claimed to be true or final. When something survives scrutiny and feels worth telling people, it gets promoted to [INSIGHTS.md](INSIGHTS.md).

---

## 2026-07-03 — Kickoff: framing the question

Seed thoughts from the opening conversation:

- The core question is **not** "how do I host a model" — it's *what does it mean to own the intelligence*, at four altitudes: nation, organization, startup, individual.
- Suspicion to test: most "sovereign AI" conversations conflate **possession** (I have weights on my hardware) with **sovereignty** (I control my dependence, my data, my capability trajectory). Are these the same? Almost certainly not. Where exactly do they diverge?
- The naive picture — "sovereignty = a local model hosted on-prem, give people access" — feels like the *minimum viable* version. What's above it? Owning the eval suite? The data flywheel? The talent? The harness/agents layer? The ability to *switch* providers at will (is exit-optionality a form of sovereignty)?
- Altitude range to cover: server/SDK-level nuances (inference stacks, deployment patterns, fine-tuning pipelines) all the way up to how intelligence ownership composes inside an org or a nation.

### Voices / theses to collect and stress-test
- **Lab leaders:** Dario Amodei (Machines of Loving Grace, compute/export-control positions), Alex Karp (Palantir's tech-republic / Western-software thesis). Add: Jensen Huang (the one who *coined/popularized* "sovereign AI" as a market), Clement Delangue (open weights as sovereignty), Arthur Mensch (Mistral's European-sovereignty pitch).
- **Policy/governance/safety:** who are the serious people here? Export-control researchers, EU AI Act architects, national AI strategy authors (India, UAE, France, Singapore, Japan…).
- **Professors/scientists:** especially domain scientists — e.g., a life-sciences researcher's version of sovereignty (data + models over proprietary lab data) is very different from a CS professor's.
- **Journalists/critics:** who is calling "sovereign AI" marketing hype? Collect the strongest contrarian takes, not the laziest.
- **Operators:** engineers, product leaders, founders, investors — what do they *do* on Monday morning if they believe in sovereignty?

### Questions with no answers yet
- Is "sovereign AI" for most nations just *buying GPUs from the same one company*? If your sovereignty runs on NVIDIA + TSMC, what did you actually gain? (The dependency just moved down the stack.)
- Is renting frontier intelligence + owning your evals/data/harness *more* sovereign than running a weaker model you fully control? (Capability vs. control trade-off — maybe the central tension of the whole project.)
- For an individual: is personal sovereignty coherent, or a romantic frame? What's the individual analog of a national compute reserve?
- Where does *open weights* actually sit? You can possess Llama/DeepSeek weights, but you didn't choose the data, can't retrain at that scale, and inherit the values baked in. Possession without reproduction capability — is that ownership?
- Time dimension: sovereignty is not a state, it's a *rate* — can you keep up? A sovereign stack that's 2 years behind frontier may be worse than dependence. Depreciation of sovereignty?

### Format notes (for myself)
- Capture conversationally — dialogues, debates, journal entries. Not tutorials, not roadmaps.
- Every candidate insight must be retellable through multiple personas: engineer, life-sciences researcher, policymaker, founder, beginner. Translation across lenses is the filter.
- Promotion bar for INSIGHTS.md: would I *tell someone this* unprompted? Does it change a decision someone would make?

---

## 2026-07-03 — Scope expansion: the technical dimensions + the method

Second pass at framing, from conversation. Two big additions: the *dimensions* the question cuts across, and the *method* for the 10 weeks.

### The technical dimensions (sovereignty is not one layer)
"Owning the intelligence" has to be interrogated across at least these axes — each one is a place where ownership can be real or illusory:

- **Infrastructure engineering** — compute, inference stacks, deployment patterns, the hardware dependency chain.
- **Context engineering** — prompts, retrieval, memory, knowledge wiring. Arguably where most *practical* ownership lives today, and the least discussed in sovereignty debates.
- **Training & post-training** — pretraining, fine-tuning, RLHF/post-training pipelines. Who can actually *shape* a model vs. merely run one?
- **Self-improvement & continual learning** — can your stack get better over time, on your data, under your control? (Connects to the "sovereignty is a rate, not a state" hypothesis above.)
- **Human–AI collaboration** — the workflows, harnesses, and judgment layers where humans and models compose. Ownership of the *collaboration pattern* may matter more than ownership of the model.
- **Security** — model security, data exfiltration, supply-chain trust, adversarial robustness.
- **Governance** — who decides, who audits, who is accountable, at every altitude from a team to a treaty.

Suspicion: the public "sovereign AI" debate lives almost entirely in the first axis (infrastructure), while the actual leverage may be distributed across all seven.

### The method: empathy first, then the problem DNA
For each dimension × altitude, the 10 weeks ask the same four questions:

1. **What exists?** — the current landscape, who's doing what.
2. **What's the frontier / state of the art?**
3. **What are the threatening problems right now?** — what do people *actually* face, not what the marketing says.
4. **What is the problem's DNA?** — the deep structure underneath. When we say "own the intelligence," it is not just having a model on-prem or trained on-prem. What is it *actually*? The goal is empathy with the people who hold the problem before proposing any answer.

### Outputs (what the scratchpad feeds)
Not just notes. The pipeline is: **scratchpad (references, links, raw learning) → patterns → storytelling**. Along the way, expect a mix of:

- **Thought experiments** — inhabiting a persona and pushing their version of sovereignty to its limits.
- **Engineering experiments** — actually building/testing something small (an inference setup, a harness, a memory store) to ground the claims.
- **Surveys** — structured landscape reviews of a dimension (e.g., the continual-learning-for-deployed-models landscape).
- **Builds** — when a question can only be answered by making something.

### Timeline, cadence, and working mode
- **Window:** ~10+ weeks, from July 3, 2026 to the first week of September 2026.
- **Cadence:** daily sessions of 60–100 minutes (100 min hard cap). Target: **100+ hours** of total human–AI collaborative work over the window.
- **Mode:** conversational learning-and-exploration, not production. I discuss, share my thought process, ask a lot of questions, and go deep; the AI's job includes **checking my assumptions and checking my understanding** — not just answering. Everything gets documented as we go.
- **Scope of any single thread:** the full causal chain — from *telemetry* (where the source data is captured) all the way to *the decision and its worldly impact*; or equivalently, from *the need/problem* to *how it gets solved* in a specific industry or country.
- **Geography is a first-class variable:** sovereign AI for the United States ≠ Europe (heavy regulatory constraints, different dependence profile) ≠ India (different scale, different government posture, different starting stack). The altitude grid isn't enough — each nation-level cell fans out by geography, which is part of why this needs 10+ weeks.
- **Possible endpoint:** if the documentation holds together, this could become a **book of sorts** — the scratchpad → insights → deep-dive-folders pipeline is effectively a manuscript pipeline.
- **Second possible endpoint — a survey paper (2026-07-05):** a proper survey of "what sovereign AI means" — to individuals, organizations, and governments/nations — doesn't exist in a rigorous form. The literature is fragmented: national strategy documents, vendor marketing, policy think-pieces, and scattered technical work that never gets composed into one map. A survey that (a) disentangles possession vs. sovereignty, (b) maps the seven dimensions × four altitudes, and (c) catalogs what's actually being built vs. claimed, could genuinely change what companies and governments think is *right to build* — the current default ("host a model on-prem") is the minimum viable version mistaken for the whole thing.
  - **Resume-trap check (per [research-engineering.md](research-engineering.md)):** the survey is only legitimate as a *harvest* of the 10 weeks, not a target that bends them. The scratchpad questions drive; if what accumulates naturally has survey shape by September, write it up. Don't run the immersion "for the paper."
  - What a survey adds that the book doesn't: citable structure for researchers/policy people, and a taxonomy others can extend. What the book adds that the survey can't: the personas, the first-person case study, the storytelling. They can share a skeleton.
  - **Refinement (2026-07-05): it's converging toward a *white paper* on sovereign AI.** That's a different genre than an academic survey, and probably the truer fit: a survey only maps what exists; a white paper *takes positions* — here's the problem, here's the landscape, here's what we found, here's what individuals/orgs/nations should actually consider building. The empathy-first method feeds the landscape half; the research-engineering probes feed the positions half (positions earned by probes, per [research-engineering.md](research-engineering.md), not asserted). Working title space: "What It Means to Own the Intelligence." Same rule still applies: harvest, not target — the genre label can keep evolving too.
  - **Settled (2026-07-05): white paper it is.** The deciding reason: it's the genre that carries *my* perception, my ideas, my thought process — a survey would launder the point of view out, and the point of view is the point. The stress-testing discipline (contrarian versions, persona translation, probes) is what keeps "my perception" from decaying into "my opinions" — the white paper argues a worldview *and* shows the work.

### The individual anchor: me
The "individual" altitude is not hypothetical — it's me, Prabakaran ([pracha.me](https://pracha.me)). This project doubles as a first-person case study: what does it concretely mean for *one person* — an AI researcher/engineer with a decision-engineering thesis — to own their intelligence stack? My own choices (what I run locally, what I rent, what I build, what memory/agents answer to me alone) become primary-source data for the individual chapter. The same question then scales up: individual → startup → enterprise → nation. The individual case is the one where I can't hide behind abstraction.

---
