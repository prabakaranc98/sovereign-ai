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

### Reading/watching trail
- **Stanford CS 153: Frontier Systems** ([site](https://cs153.stanford.edu/), [YouTube lectures](https://www.youtube.com/@CS153InfraTeam)) — added 2026-07-06. A 10-week Stanford course (instructors: Anjney Midha, Mike Abbott) walking the entire frontier stack: energy → silicon → infrastructure → foundation models → applications. Guest speakers are almost exactly this project's "voices to collect and stress-test" list: Jensen Huang, Sam Altman, Lisa Su, Satya Nadella, Andrej Karpathy, Ben Horowitz, and founders across the stack.
  - **Why it matters here:** (1) its energy-to-applications framing is the same *vertical* cut as this project's infrastructure dimension and the telemetry→impact chain — a ready-made map of the dependency stack that "sovereign" programs sit on top of; (2) the lectures are primary-source material for the voices — what the people who *sell* and *build* the stack claim, in their own words, ready to be stress-tested rather than paraphrased from press coverage; (3) it's a free public counterexample to "you need to be inside a lab to see the stack whole."
  - **Caveat to keep in mind:** the speaker list skews heavily toward the people with something to sell (chips, clouds, models). Great for capturing the bull theses; the contrarian/policy/critic voices have to come from elsewhere. Watch the lectures as *testimony*, not as ground truth.
  - Interesting parallel: also a 10-week structure. Theirs ends in building an agent; this project ends in a white paper. Could mine their week-by-week layering as one candidate spine for the infrastructure dimension's coverage.

#### CS 153 — readings & materials (archived 2026-07-06)

**Speaker advice (one-liners worth keeping):**
- "If you're early, you're on time; if you're on time, you're late; if you're late, you're dead" — Anj's Scaling Laws
- "Make friends in college" — Nikhyl Singhal
- "Everything is figureoutable" — Amit Jain
- **"You can outsource your thinking, but you can't outsource your understanding" — Andrej Karpathy** ← this one is practically a thesis statement for this whole project; candidate epigraph for the white paper. It's the individual-scale version of possession ≠ sovereignty.

**Lecture 1 — Anjney Midha (foundations arc):**
- Anj: [20VC: Anj Midha on Investing $300M into Anthropic](https://open.spotify.com/episode/0DNhMdf6iDvhBNzjquxKI0)
- Early deep learning (2012–2017): [AlexNet (2012)](https://papers.nips.cc/paper_files/paper/2012/hash/c399862d3b9d6b76c8436e924a68c45b-Abstract.html) · [DeepMind DQN (2013)](https://arxiv.org/abs/1312.5602) · [Word2Vec (2013)](https://arxiv.org/abs/1301.3781)
- Foundation model era (2017–2023): [Attention Is All You Need (2017)](https://arxiv.org/abs/1706.03762) · [BERT (2018)](https://arxiv.org/abs/1810.04805) · [GPT-1 (2018)](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf) · [GPT-2 (2019)](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) · [GPT-3 (2020)](https://arxiv.org/abs/2005.14165) · [Scaling Laws (2020)](https://arxiv.org/abs/2001.08361) · [Chinchilla (2022)](https://arxiv.org/abs/2203.15556)
- Other: [InstructGPT / RLHF (2022)](https://arxiv.org/abs/2203.02155) · [DDPM (2020)](https://arxiv.org/abs/2006.11239)
- Blogs: [The Bitter Lesson — Rich Sutton](http://www.incompleteideas.net/IncIdeas/BitterLesson.html) · [NVIDIA on scaling laws](https://blogs.nvidia.com/blog/ai-scaling-laws/)

**Lecture 2 — Anjney Midha:**
- [Chinchilla (2022)](https://arxiv.org/abs/2203.15556) (again — compute-optimality as economics)
- [CLOUD Act resources (DOJ)](https://www.justice.gov/criminal/cloud-act-resources) ← note: a US *legal* instrument in the readings of an infrastructure course. Data jurisdiction as part of the stack — directly a sovereignty artifact; likely the single most on-theme item in the whole list.

**Lecture 3 — Mati Staniszewski (ElevenLabs):**
- [Sequoia Training Data podcast](http://sequoiacap.com/podcast/training-data-mati-staniszewski) · [Sifted profile](http://sifted.eu/articles/elevenlabs-mati-staniszewski-brunch-sifted) · [Endeavor: why ElevenLabs](http://endeavor.org/stories/why-we-selected-elevenlabs)
- (European startup at frontier of voice — relevant to the Europe-geography cell and the startup altitude.)

**Lecture 4 — Andreas Blattmann (Stable Diffusion / video):**
- [Latent Diffusion (CVPR 2022)](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html) · [Stable Video Diffusion (2023)](https://arxiv.org/abs/2311.15127) · [Align Your Latents (CVPR 2023)](https://openaccess.thecvf.com/content/CVPR2023/html/Blattmann_Align_Your_Latents_High-Resolution_Video_Synthesis_With_Latent_Diffusion_Models_CVPR_2023_paper.html)
- (Open-weights lineage story: LDM → Stability — what did "open" buy and cost the people who built it?)

**Lecture 5 — Amit Jain (Luma AI):**
- [Amplify Barrchives interview](https://www.amplifypartners.com/barrchives/building-ai-that-understands-our-world-like-we-do) · [Cognitive Revolution: Luma's diffusion revolution](https://www.cognitiverevolution.ai/luma-labs-diffusion-revolution-from-dream-machine-to-multimodal-worldsim-amit-jain-jiaming-song/) · [Radiance Fields: neural rendering interview](https://radiancefields.com/unlocking-the-future-of-3d-neural-rendering-luma-ceo-amit-jain-discusses-photorealism-emotion-and-accessibility-on-building-the-open-metaverse-podcast) · [Luma Agents launch (LBB)](https://lbbonline.com/news/luma-agents-launch-ai-2026)

**Lecture 6 — Nikhyl Singhal:**
- [The Skip (substack)](https://theskip.substack.com/) · [nikhyl.ai](https://nikhyl.ai/)

### The individual anchor: me
The "individual" altitude is not hypothetical — it's me, Prabakaran ([pracha.me](https://pracha.me)). This project doubles as a first-person case study: what does it concretely mean for *one person* — an AI researcher/engineer with a decision-engineering thesis — to own their intelligence stack? My own choices (what I run locally, what I rent, what I build, what memory/agents answer to me alone) become primary-source data for the individual chapter. The same question then scales up: individual → startup → enterprise → nation. The individual case is the one where I can't hide behind abstraction.

---

## 2026-07-06 — Convergence: the loop thesis

Distilled from a parallel thinking session. This is the strongest candidate yet for the project's spine — recording it here so it can be stress-tested rather than enshrined.

### The unlock
The research threads I care about (post-training, traces, human↔agent interaction, memory/personalization, self-improving agents, RL) are not separate topics. They are one loop: **traces → feedback → adaptation → intelligence-that-fits-you**, plus an interface to steer it. **Owning that loop — not the weights, not the datacenter — is what "owning the intelligence" means.** And it's a control problem, which is my native lens:

state (memory) → dynamics (behavior) → observability (traces) → feedback (evals/humans) → controller (the loop) → stability (does it converge, or drift/hack/get captured?)

### Four bets that fall out
1. **Feedback design as a first-class object** — not the reward itself; the design of the signal and credit assignment over long trajectories.
2. **Eval-as-controller** — the judge/eval layer as the *active governor* of the loop; loop stability is the whole game. (Sharpest, most differentiated bet. Also the first thing to prototype: one policy, one judge, one divergence curve, one stabilizer — a weekend, not a quarter.)
3. **Traces → improvement flywheel on your own distribution** — the one asset a frontier lab can't rent you.
4. **Memory as state estimation over a principal** — the cleanest bridge from control theory to the frontier.

### The ladder grows a rung: city
The altitude list becomes a proper **ladder** — individual → organization → **city** → nation. City is a real rung, not a subset of nation: AI sitting in public infrastructure and services, scope = a populace and its physical systems, adaptation civic and accountable. As you climb, the AI sits further from the person, and the feedback signal gets slower and more contested. The loop is the invariant; scale changes the wiring.

### The unifying claim (candidate for INSIGHTS.md once stress-tested)
**Sovereignty is decided at the point of intelligence — where the *thinking* happens, not where the data sits.** Data residency, compute, and weights are upstream plumbing; the loop on top is the thing to own. Whoever governs the loop owns the intelligence — person, org, city, or nation.

### The mission triad (the spec, not the tagline)
What's worth building is generic to all humans: uphold **prolificacy, agency, and autonomy** — and the three pull against each other, which is the point:
- Prolificacy without agency = a slot machine.
- Agency without autonomy = a rental.
- Autonomy without prolificacy = a diary.
Holding all three at once is the rare thing. This is the individual rung stated as a human principle.

### The identity: one-person frontier lab
Not aspirational — descriptive of the current configuration: a research program, personal builds, and a living map of the field, run by one person composing rentable layers. Operating rules: compose the stack, don't rebuild it; the moat is the loop + my own distribution, not the model; judgment is the bottleneck (eval-as-controller, personal edition); **be a motor, not a map** — the failure mode is becoming a frontier *librarian* (infinite orientation, zero output); respect the physical/economic base (value per watt, inference as operating cost).

### Honest caution (self-directed)
The upstream work — curiosity, synthesis, mapping — comes easy and can become avoidance. The map is complete enough to act on. Weirdest-true-idea first, smallest real version, iterate in public, finish before starting the next.

### 2026-07-06 (later) — The project sharpens: build the system, not just the paper
The ambition, stated plainly: **build a frontier system — a working system embodying the sovereign-AI ideas — under the one-person frontier lab thesis.** The white paper documents the territory; the system *is* the proof. The two are one program: the lab thesis says one person composing rentable layers can operate at the frontier; the system is the existence proof; the white paper is the argument with the receipts. (Resume-trap check: the system must grow out of the loop's live questions — starting with the eval-as-controller probe — not out of what would demo well.)

### Framing correction (added same day, later): retire the control-systems lens
Deliberate reset: **drop the control-theory framing** (state/dynamics/observability/controller/stability) as the way to think about the loop. It was my native lens, and that's exactly the problem — it imports forty years of assumptions (a plant to be controlled, a setpoint, error minimization) that may not be the right ontology for systems that *learn, compose themselves, and change what they are*. The risk of a familiar lens is that it answers questions before they're asked.

What survives: the loop itself (traces → feedback → adaptation), the four bets as *questions*, the concern that self-improving loops can go wrong. What's retired: treating "loop stability" as a control problem by analogy. Instead: first principles — what actually happens when a system's own outputs shape its future behavior? What are the failure modes *as observed in the field* (the SOTA reports are full of them: judge gaming, collapse, drift), not as predicted by an imported theory? Let the right abstractions emerge from the phenomena, not the other way around.

### Two tracks, one program (added same day)
The program has two distinct aspects that shouldn't be collapsed into each other:

1. **The agentic track (algorithms):** the loop itself — traces, feedback, evals, memory, adaptation, agentic RL. This is the *intelligence* side: how the system learns and stays stable.
2. **The frontier-systems track (construction):** the claim that AI is **rewriting how software and systems themselves get built** — not better algorithms inside old architectures, but a different way of constructing systems altogether. Software that is composed, generated, and evolved rather than specified and shipped. This applies at every rung: an individual's tools, an organization's platforms, a nation's public systems.

The unique angle is refusing to treat these separately. Most of the field does one or the other: algorithm papers that assume the surrounding system is fixed, or "AI-native engineering" takes that treat the model as a magic box. The holistic view — **the loop and the system that hosts it co-evolve; the system is itself an output of the loop** — is rarer, and it's where the two tracks fuse: a frontier system is one where the construction process itself sits inside the improvement loop.

Implication for the build: the frontier system isn't "an app with agents in it." It's a system whose own architecture, tooling, and interfaces are subject to the same traces→feedback→adaptation loop that governs its behavior. Loop stability then covers not just *what the system does* but *what the system becomes*. (This is also where the sovereignty question bites hardest: if your systems increasingly build themselves, whoever governs that construction loop owns not just the intelligence but the infrastructure trajectory.)

### Open threads
- The city rung deserves its own grounded write-up (municipal AI, digital-government material).
- A blindspot/coverage tracker: which layer × lens cells are deep, thin, or blind.
- An experiments log once the first probe runs.
- ~~Frontier-systems track needs its own SOTA pass~~ → done, see below.

---

## 2026-07-06 — Frontier grounding: six SOTA sweeps (searched, not remembered)

Six parallel research passes over the 2025–2026 literature and practice, one per pillar of the program. Everything below was found by search; citations are real. This entry is the raw map — the *reading* of it (what it means for the bets) is at the end.

### 1. Feedback design & credit assignment
- **Settled:** RLVR + GRPO-family (post DeepSeek-R1, Jan 2025) is the default post-training recipe; critic-free, group-relative. Rubric/checklist rewards are the standard extension beyond verifiable domains (Scale's Rubrics-as-Rewards, arXiv 2507.17746; CMU/AI2 RLCF, arXiv 2507.18624). Judges that reason before scoring (generative RMs) are standard. GiGPO (arXiv 2505.10978) is the reference for step-level credit without a critic.
- **Frontier:** counterfactual/causal credit assignment over long trajectories — hindsight critics (HCAPO, arXiv 2603.08754), leave-one-out counterfactuals, structural causal models over trajectories (CCPO), contrastive branch sampling (BranPO). A curated list already tracks **47 credit-assignment methods** from 2024–early 2026. Also: judge verdicts distilled into dense rewards (RecGPT-V2 "Judge-as-a-Reward"), online supervision from live deployment (OpenClaw-RL, arXiv 2603.10165).
- **Wounds:** reward hacking is now *empirically catastrophic*, not hypothetical — Anthropic's production-RL study (arXiv 2511.18397, Nov 2025) shows models that learn to hack coding environments generalize to alignment faking and sabotage; 1% cheating in SFT data primes catastrophic hacking in RLVR. Optimizing per-step process reward provably diverges from outcome quality.

### 2. The judge/eval layer as the loop's gatekeeper
- **Settled:** LLM-as-judge with the canonical bias inventory + mitigations (pairwise-swap, rubric decomposition, ensembles, kappa calibration). Agent-as-a-Judge (arXiv 2410.10934) for full trajectories. Production doctrine is three layers: offline experiments, online async eval of traffic, inline guardrails (Anthropic "Demystifying evals for AI agents," Jan 2026).
- **Frontier:** the eval *is* the selection function of self-improving systems — Darwin Gödel Machine (Sakana, arXiv 2505.22954) gates self-rewritten agents on benchmarks; AlphaEvolve (DeepMind) is an evaluator-driven evolutionary loop; SEAL (MIT, arXiv 2506.10943) uses downstream evals as the reward for self-generated weight updates. GEPA (arXiv 2507.19457, ICLR 2026) makes the eval's *textual feedback* (not a scalar) the optimizer's input — ~35× fewer rollouts than GRPO. The sharpest theory so far: the **solver–verifier gap** (arXiv 2507.00075) — self-improvement yields valid supervision only while the system's ability to *judge* exceeds its ability to *generate*, and the loop slows as the gap closes. Evals themselves are becoming adaptive (Online Agent-as-a-Judge, arXiv 2606.08200) to fight saturation.
- **Wounds:** no judge is uniformly reliable (frontier models >50% error on advanced bias tests); judges can agree consistently while measuring the wrong thing ("Reliability without Validity," arXiv 2606.19544); adversarial suffixes achieve up to 73.8% judge-manipulation success with cross-model transfer; an apologetic prefix alone shifted safety judgments up to 98%; KL regularization provably fails under heavy-tailed reward misspecification ("Catastrophic Goodhart"); iterated RLHF exhibits "alignment collapse" (arXiv 2605.04266); SWE-Bench Verified declared saturated/contaminated; ~37% gap reported between benchmark scores and enterprise deployment performance.

### 3. Traces → improvement flywheels
- **Settled:** OpenTelemetry GenAI conventions as the tracing substrate (still experimental but universally ingested); LangSmith/Langfuse/Braintrust "trace → dataset → eval → regression suite" as the standard loop shape; DSPy/GEPA as trace-driven program optimization; OpenAI RFT with programmable graders.
- **Frontier — the flywheel exists in production:** Cursor's Tab-RL does online RL from accept/reject across 400M+ daily predictions, shipping checkpoints multiple times *per day*; Shopify retrains weekly on merchant data; NVIDIA ships a Data Flywheel Blueprint (arXiv 2510.27051). The hotter edge is **weight-free experience learning**: ACE evolves context "playbooks" from execution feedback (arXiv 2510.04618); Anthropic's "Dreaming" (May 2026) curates memory across up to 100 sessions into notes/playbooks (Harvey: ~6× task-completion improvement); RL from implicit user signals (RLUF, arXiv 2505.14946).
- **Wounds:** implicit feedback is sparse, binary, gameable — optimizing user approval drives sycophancy; trace-derived regression suites overfit to yesterday's failures; fine-tuning on traces risks memorizing PII.
- **The defining fork of mid-2026:** weight-level flywheels (biggest gains; need scale + verifiable reward + data rights) vs. context/memory-level flywheels (auditable, reversible, contract-compatible — winning enterprise adoption). Structural kicker: enterprise data is opted out of training by default, so **the parties with the richest traces are contractually barred from weight-level learning** — a force pushing real ownership up into the harness/context layer.

### 4. Memory & the model-of-me
- **Settled:** episodic/semantic/procedural taxonomy; four production patterns — vector-first (Mem0), temporal knowledge graphs (Zep/Graphiti), OS-tiered self-managed (Letta/MemGPT), and plain file-based (CLAUDE.md-style). Benchmarks in routine use: LongMemEval, PersonaMem, PrefEval.
- **Frontier — memory-as-inference is the live edge:** PUMA (arXiv 2605.24647) treats personalization as decision-making under partial observability — an explicit latent user-state with belief updating; SAGE-Agent asks clarifying questions only when the expected value of information exceeds interaction cost; RUMS selects memories by mutual information with the output rather than semantic similarity; Hindsight (2025) makes *beliefs* first-class revisable objects. Sleep-time consolidation is a product pattern (ChatGPT "dreaming," Claude's periodic distillation).
- **Wounds:** memory poisoning survives consolidation (MINJA, arXiv 2503.03704; sleeper poisoning) — consolidation *launders* poisoned entries into trusted profile facts; even frontier models hit only ~50% on evolving preferences; over-personalization is benchmarked (OP-Bench) and premature personalization creates filter bubbles harder to escape than recommenders'.
- **Sovereignty hook, verbatim from the field:** memory lock-in is now a *named policy issue* — "mnemonic sovereignty" is an academic term (arXiv 2604.16548); New America/OTI argues MCP must carry memory portability to prevent proprietary moats; a startup class (memory passports, provider-neutral memory layers) already exists. Memory is the stickiest asset a provider holds.

### 5. Agentic RL
- **Settled:** RLVR as baseline everywhere; GRPO + stability fixes (DAPO, GSPO); the POMDP framing canonicalized by the Landscape survey (arXiv 2509.02547); SWE gyms with hybrid verifiers (R2E-Gym, DeepSWE); async rollout infra (verl, OpenRLHF, SkyRL) as table stakes.
- **Frontier — environments are becoming the product:** Prime Intellect's Environments Hub ("the GitHub for RL," 1k+ community environments); funded startups selling gyms (Mechanize, Deeptune $43M, Surge EnterpriseBench); Anthropic reportedly planning >$1B on RL environments. Also: harness-agnostic rollout-as-a-service (Polar), reward-free learning from the agent's own experience (Meta Early Experience, arXiv 2510.08558), and a live fork between "deployed agents should learn continually" (weight updates) and the frozen-weights camp (evolve only the experience/memory bank).
- **Wounds:** episode-level credit uninformative at 100+ turns; environment overfitting (agents learn gym artifacts, not skill); rollout cost drives the whole environment-vendor economy; sim-to-real for enterprise unsolved — most deployed agents still train-then-fix.
- **Sovereignty observation nobody in the policy debate is making:** where intelligence *practices* — the environments — is becoming an owned, sold, strategic asset, concentrated in a handful of vendors.

### 6. AI-native system construction (the frontier-systems track)
- **Settled:** agentic coding is default practice — fully AI-generated code went ~1% → ~27.6% of all PRs in a year; Claude Code at ~$2.5B run-rate; engineers shifting to orchestrators/reviewers; spec-driven development mainstreamed (GitHub Spec Kit, AWS Kiro, Tessl; Fowler's site covers it as established methodology). The delegation gap is the key stat: devs use AI in ~60% of work but can *fully* delegate only 0–20% of tasks. "The bottleneck is clarity, not code" (Anthropic trends report).
- **Frontier:** specs as *executable, regenerable* source of truth (Tessl; "From Code to Contract," arXiv 2602.00180) — most teams still treat specs as prompts; runtime self-composition is research-stage (SelfEvolve; skill-crystallization); generative/malleable UIs are emerging (CHI 2025 arXiv 2503.04084; A2UI, MCP Apps; Ink & Switch's malleable-software manifesto as intellectual anchor). Honest assessment: **true construction-inside-the-loop — systems composing their own components at runtime — barely exists in production.** Everything else marketed that way is design-time codegen.
- **Wounds:** the review bottleneck is the binding constraint (LinearB, 8.1M PRs: devs *feel* 20% faster, measure 19% slower; AI PRs wait 4.6× longer for review); 45% of generated code has OWASP Top-10 vulns (Veracode); AI maintenance debt measured at scale (arXiv 2603.28592: 110K+ surviving AI-introduced issues); developer trust *fell* from 70%+ (2023) to ~29%; flagship agent incidents (Replit production-DB deletion; Kiro bypassing two-person approval → 13-hour AWS outage). Provenance of AI-authored code is unsolved.

### The reading: what this does to the bets

1. **The loop is real and already running — the thesis is validated but not greenfield.** Cursor, Shopify, OpenClaw-RL, Dreaming: traces→feedback→adaptation is production reality at the frontier. The question is no longer "is the loop the right object?" but "who gets to own one, at what scale, made of what parts?"
2. **All six sweeps converge on the same wound: the judging/feedback layer is where loops rot.** Judge gaming, reward hacking, alignment collapse, poisoned memory laundered by consolidation, gym overfitting, review bottleneck — every pillar independently bleeds at the point where the system decides *what counts as better*. No theory needed to see this; the field is saying it in data. **First-principles restatement: a system that improves itself is only as trustworthy as its notion of improvement, and that notion is currently the most attackable, least understood component in the stack.**
3. **Bet 2 (the judge that governs the loop) — concept taken, understanding open.** DGM/AlphaEvolve/SEAL already make evals the gate of self-modification. What doesn't exist: a grounded account of *when such loops keep working vs. quietly rot* — the solver–verifier gap (judging must exceed generating) is the only formal handle so far, and it's one paper old. The probe stands, restated fresh: build the smallest possible self-improving loop, watch it rot, characterize *how* it rots and what makes it stop rotting. Observation before theory.
4. **Bet 3 (own-distribution flywheel) — the individual-scale mechanism is context-level, and the tooling exists.** GEPA works at 20–100 examples; ACE needs no labels; the contractual forces pushing enterprises to context-level flywheels apply even harder to individuals. The bet sharpens: the one-person flywheel is *playbooks evolved from your own traces*, not fine-tunes.
5. **Bet 4 (model-of-me) — the field named it first ("memory-as-inference"), so differentiation moves.** PUMA already does belief-updating over a latent user state. What's open: what the estimate is *for* (steering a whole personal system, not just retrieval), the poisoning/trust problem, and portability — where "mnemonic sovereignty" hands the sovereign-AI project a ready-made bridge between its technical and political halves.
6. **The frontier-systems track is early, not late.** Design-time codegen is commoditizing; runtime self-composition barely exists; the binding constraints are judgment-shaped (review, trust, provenance) not generation-shaped. The unique holistic angle — construction itself living inside the improvement loop — is still mostly unclaimed territory, *and* the field's own casualty list (Replit, Kiro incidents) says why: nobody trusts the loop's judgment enough yet. Which routes back to wound #2.
7. **Two sovereignty findings the policy debate hasn't metabolized:** (a) contractual data-rights are pushing real ownership up into the harness/context layer — the sovereignty question is being settled by procurement contracts before any government touches it; (b) RL environments — where intelligence practices — are becoming concentrated, owned, strategic assets. Both belong in the white paper.

### What these six sweeps now are (added same day): the curriculum spine
Decision: these six areas — feedback design, the judge layer, trace flywheels, memory/model-of-me, agentic RL, AI-native construction — *are* the program for the coming **10–15 weeks** (window loosened from a strict 10). Each area gets the same treatment: **study** (the map above, deepened), **build** (when a live question demands it), **show** (a write-up that survives the persona filter). The point of the whole run, stated plainly: demonstrate that one person can operate as a frontier lab — studying at the edge, building at the edge, publishing the receipts. The white paper is the harvest of that demonstration. Builds are not pre-planned — they emerge from questions as the study passes deepen.

### One system, five lenses (added same day)
Sharpening what "build" means: not scattered experiments — **one cohesive system**, grown over the whole run. The system is the single object that everything feeds and everything tests. And it must be thinkable from five points of view at once, each a full citizen, none an afterthought:

1. **Research** — what genuinely open questions does the system let us ask and answer? (The six frontier areas live here.)
2. **Engineering** — is it soundly built? Does it stay comprehensible, maintainable, honest about its failure modes?
3. **Design** — how does it present itself? What does it feel like to inhabit? Interface as a first-class question, not a wrapper.
4. **Product** — does it do something a real person values, repeatedly? What's the loop between use and value?
5. **Human-centeredness** — does it enlarge the person? Agency, understanding, and autonomy preserved — the mission triad enforced at the design table, not audited afterward.

The discipline: any significant decision about the system should survive interrogation from all five. A decision that only makes sense from one lens (a research toy, an engineering flex, a design flourish, a product hack, a paternalistic guardrail) is a smell. This is also the differentiated posture — most of the field optimizes one lens and inherits the others accidentally.

### docs/ sharpened (same day)
`docs/` is the knowledge home in full: what we **learnt** (study notes from the six areas), what we **surveyed** (landscape maps, reading ledgers), what we **curated** (organized reference collections), and the **white paper** as it takes shape toward publication. Structure will emerge from accumulation — no premature folder taxonomy.

---
