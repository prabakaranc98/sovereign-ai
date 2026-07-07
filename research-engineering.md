# Research Engineering — what it means to this repo

> A working definition, not a settled one. This file exists because "research engineering" is the *method* of this project, the same way [SCRATCHPAD.md](SCRATCHPAD.md) is its workbench. It will get revised as the practice reveals itself.

## The short version

**Research engineering is how claims about sovereignty get earned instead of asserted.**

This repo asks "what does it mean to own the intelligence?" That question can be answered two ways: by collecting opinions, or by *touching the stack* — running the model, building the harness, measuring the gap, feeling where ownership is real and where it's a brochure. Research engineering is the second way. It's the discipline of converting a belief into an experiment small enough to run in a 100-minute session and honest enough to change your mind.

## Why this project needs it

The sovereignty debate is saturated with claims made from altitude — keynotes, national strategies, funding announcements. Almost nobody making those claims has recently:

- stood up an open-weights model and measured what it actually costs to keep it *competitive*, not just running;
- tried to move a real workload between providers and timed how long "exit optionality" actually takes;
- built a memory/context layer and tested whether it survives a model swap (is the harness really where ownership lives?);
- fine-tuned on proprietary data and checked whether the resulting capability is *durable* or evaporates at the next base-model release.

Every one of those is a sovereignty claim wearing an engineering costume. Research engineering is what lets this repo say "we checked" instead of "we read that."

## What it means at each altitude

The method scales the same way the question does:

- **Individual** — the most direct: my own stack *is* the lab. What I run locally, what I rent, what breaks when I switch — first-person telemetry. No abstraction to hide behind.
- **Startup / org** — mostly reconstructable: the experiments are small-scale replicas of enterprise decisions (host vs. rent, fine-tune vs. context-engineer, one provider vs. an abstraction layer), plus reading engineering postmortems as data.
- **Nation** — not runnable, but still *engineerable*: the research-engineering move here is decomposition and estimation — take a "sovereign AI program" announcement apart into its bill of materials (compute, energy, talent, data, dependence graph) and check whether the numbers and dependencies close. Fermi engineering as a truth filter.

## The practice (rules of thumb for this repo)

1. **Every big claim gets a smallest-possible probe.** Before an idea is promoted to [INSIGHTS.md](INSIGHTS.md), ask: what is the cheapest experiment, measurement, or decomposition that could embarrass it? If we can't name one, the idea isn't stress-tested yet.
2. **Build to learn, not to keep.** Artifacts here are instruments, not products. A throwaway harness that settles a question beats a polished repo that doesn't.
3. **Measure the *rate*, not the state.** Since a core hypothesis is that sovereignty is a rate (can you keep up?), experiments should where possible capture change over time — cost drift, capability gap vs. frontier, migration friction — not one-shot snapshots.
4. **Log negative results in the scratchpad.** An experiment that kills a nice hypothesis is a better output than one that flatters it. The scratchpad is where hypotheses go to be wrong safely.
5. **The write-up is part of the experiment.** If the result can't be retold across the personas (engineer, scientist, policymaker, founder, beginner), the experiment isn't finished — it's just done.

## The anti-pattern: the resume trap

A standing guardrail, from [Curriculum as a Living System](https://pracha.me/musings/posts/2026_07_03_curriculum-as-a-living-system.html#resume-trap): the failure mode where projects get reverse-engineered from what will *look* like a match — a job description, a trend, an imagined reader — and assembled backward from external criteria. The output technically checks the box but develops no taste, no depth, and converges on the same generic demo everyone else built.

Applied here, the trap has a specific local form: **running experiments because they'd look good in the book, rather than because a live question demands them.** A "sovereignty benchmark" built for optics is exactly as hollow as a portfolio project built from a job posting. The tell is directionality:

- **Trapped:** "what experiment would make this chapter impressive?" → build → retrofit a question.
- **Alive:** a genuine question surfaces in the scratchpad → it resists armchair resolution → the *smallest probe that could embarrass it* gets built.

Every experiment in this repo must be traceable back to a scratchpad entry that existed before the experiment did. If the question can't be found upstream of the build, the build is decoration — cut it. This is also why the curriculum here stays *living*: the 10-week plan is a commitment to depth, not a syllabus to be covered, and the experiment list is allowed (expected) to be rewritten by what the early probes find.

## Relationship to the rest of the repo

- **[SCRATCHPAD.md](SCRATCHPAD.md)** supplies the hypotheses; this practice supplies their trials.
- **[INSIGHTS.md](INSIGHTS.md)** — its promotion bar ("stress-tested") is, in practice, mostly a research-engineering bar: has the strongest version of the claim survived contact with a probe?
- **Engineering experiments** (from the outputs list in the scratchpad) are this file's method applied; thought experiments are its cheaper sibling — same rigor, run in the head instead of on the machine.

---

*A live definition. Started July 2026; expected to be wrong in interesting ways by September.*
