# AI with Ravi — Friday Evening Edition
## X/Twitter Briefing · March 27, 2026 · Last 12 Hours

*Curated for longer-term value and learning edge — not the flashy stuff.*

---

## 1. The Economics of Reasoning Models Has a Dirty Secret

**lingjiao chen @ChenLingjiao · 5h** *(reposted by James Zou @jmzou1)*

A Stanford / UC Berkeley / CMU / Microsoft Research paper exposes what they call the **"Price Reversal" phenomenon** in Reasoning Language Models: in 21.8% of model-pair comparisons, the model with the *lower* listed API price actually costs *more* in practice. The culprit is thinking tokens — one model can consume 900% more thinking tokens than another on the identical query. The paper evaluated 8 frontier RLMs across 9 task categories including competition math, science QA, code generation, and reasoning. The key finding: removing thinking token costs from the ranking reduces reversals by 70% and raises the price-performance correlation from 0.563 to 0.873. Listed API pricing is not a reliable proxy for actual inference cost, and per-query cost prediction is "fundamentally difficult" because repeated runs of the same query yield thinking token variation up to 9.7×. The practical takeaway for anyone selecting models for production: sticker price is close to meaningless without per-query token profiling.

*[@ChenLingjiao](https://x.com/ChenLingjiao) · 5h · 4.1K views · reposted by [@jmzou1](https://x.com/jmzou1)*

---

## 2. Reading the Chain of Thought Does Not Solve Interpretability

**Riya Tyagi @riyatyagi86 · 2h** *(amplified by Neel Nanda @NeelNanda5 · 1h)*

The interpretability community has been wondering whether simply reading an AI's chain of thought (CoT) constitutes meaningful interpretability. Riya Tyagi and Neel Nanda's answer: no, and they've built 9 hard tasks to prove it. The tasks are designed so that reading the CoT does not reveal the answer — you need to know the *true* ground truth independently. The research highlights a structural problem: it's surprisingly difficult to prove that CoT monitoring has *failed*, because any monitoring method that looks at the chain of thought output is subject to the same limitation — the model could be hiding its actual reasoning in the underlying computation rather than exposing it in the visible scratchpad. This is a call to develop mechanistic interpretability tools that go beyond surface-level text output. Neel Nanda: "It's surprisingly hard to tell if you have made progress on interpreting reasoning models."

*[@riyatyagi86](https://x.com/riyatyagi86) · 2h, amplified by [@NeelNanda5](https://x.com/NeelNanda5) · 1h*

---

## 3. The Intelligence Explosion Will Be Collective, Not a Single Mind

**elvis @omarsar0 · 1h** *(sharing Google DeepMind paper)*

A new Google paper — "Agentic AI and the Next Intelligence Explosion" — makes a foundational argument that challenges the dominant narrative about superintelligence. The paper's central claim: every prior intelligence explosion in human history (language, writing, science, industrialization) was *social*, not individual. The AI "singularity" imagined as a single superintelligent mind bootstrapping to godlike intelligence is, the authors argue, fundamentally wrong. What's actually emerging is plural, distributed, and organizational: AI reasoning models already spontaneously generate "societies of thought" internally through multi-agent dynamics — exhibiting specialization, hierarchy, division of labor, and structured disagreement. The paper calls for research into how AI groups exhibit these social dynamics and what makes human-agent social reasoning grounded and durable. The implication: the interesting unit of analysis is not the individual model's capability but the architecture of collective AI cognition.

*[@omarsar0](https://x.com/omarsar0) · 1h · 4.2K views*

---

## 4. Autoresearch Finds 20 Improvements That All Transfer Across Model Scale

**AVB @neural_avb · ~15m** *(citing Andrej Karpathy @karpathy, Mar 9)*

Andrej Karpathy left autoresearch running on nanochat (a depth=12 model) for two days. It found approximately 20 changes that each improved validation loss. When Karpathy manually tested every single one, all of them were additive and *all transferred* to the larger depth=24 model. This is the key result that hasn't been emphasized enough: algorithmic improvements discovered by automated research at small scale generalized to a 2× larger architecture without any human curation or cherry-picking. AVB's follow-up question — "if someone were to cite autoresearch in a research paper, would they just paste the URL of this tweet?" — points to a genuine coming crisis in attribution, reproducibility, and credit in AI research as automated systems begin producing citable scientific results.

*[@neural_avb](https://x.com/neural_avb) · ~15m, citing [@karpathy](https://x.com/karpathy) · Mar 9*

---

## 5. A Doctor Quits Peer Reviewing Because AI Is Better at It

**Derya Unutmaz, MD @DeryaTR_ · 4h**

Derya Unutmaz has announced he will no longer accept requests to review scientific papers, for a principled reason: current top AI models do a better job than he can for more than 95% of the review process. "With less than 5% effort, it would not be fair for me to take credit, and journals don't like it anyway." This statement has significant institutional weight — Unutmaz is an immunologist and professor, not a junior researcher feeling imposter syndrome. The same thread links to Jason Locasale's @LocasaleLab observation that a paper took nearly 3 years from submission to publication, while many academics still won't consider work "real" if it appears first as a preprint. Together these paint a picture of a peer review system simultaneously too slow to be useful and too manual to survive contact with AI.

*[@DeryaTR_](https://x.com/DeryaTR_) · 4h · 19K views, 328 likes; [@LocasaleLab](https://x.com/LocasaleLab) · 4h*

---

## 6. Claude Code Hooks: The Difference Between Suggestion and Guarantee

**Akshay @akshay_pachaar · 7h**

The most practically useful technical thread of the day: Akshay explains Claude Code's Hooks system with a framing that cuts through the noise. "CLAUDE.md is just a suggestion. Hooks are a guarantee." The distinction matters because Claude follows CLAUDE.md *most* of the time — but not all of the time. Hooks intercept tool calls at two checkpoints: **PreToolUse** (a security gate that can block execution before the tool runs) and **PostToolUse** (a formatter that cleans output after execution). There are three exit codes: 0 means proceed, 1 means error but Claude continues anyway, 2 is the only one that actually blocks execution. Use cases shown: custom logging/analytics, scanning prompts to block accidentally pasted API keys, auto-summarizing conversations to create persistent memory, running a custom validator when a conversation turn stops, customizing prompting per directory. Hooks are behind a feature flag: `[features] codex_hooks = true`. This changes the mental model of Claude Code from "AI you instruct" to "AI runtime you can program."

*[@akshay_pachaar](https://x.com/akshay_pachaar) · 7h · 5.1K views*

---

## 7. Attention as Selective Memory: Kimi's New Architecture

**Rohan Paul @rohanpaul_ai · 1h** *(featuring Yang Zhilin, CEO Moonshot AI / Kimi)*

Yang Zhilin, founder and CEO of Moonshot AI (the Chinese lab behind Kimi), gave a talk on a new architecture concept: **Attention Residuals**. The core argument is about what attention *should* do: not mechanically store everything, but selectively retain what matters. The framing reframes attention from a retrieval mechanism to a memory curation mechanism — a model keeps the residue of what it found important, rather than maintaining equal fidelity to all inputs. This connects to a long-standing question in architecture research about whether transformers' attention is fundamentally wasteful, and whether something closer to biological selective attention would yield better efficiency and generalization. Moonshot AI released a new architecture yesterday alongside this talk.

*[@rohanpaul_ai](https://x.com/rohanpaul_ai) · 1h · 3.1K views (Kimi.ai video)*

---

## 8. One Pet Owner, No Biology Background, Custom mRNA Cancer Vaccine

**Paul Conyngham @paul_conyngham · Mar 25** *(surfaced by @DeryaTR_ · 2h)*

Paul Conyngham — not a biologist, not a doctor — documented how he used AI to design a custom mRNA vaccine protocol for his dog Rosie's cancer. The article "How I created Rosie's mRNA Vaccine Protocol" is being called by Derya Unutmaz "one of the historical inception stories in the age of AI." The pattern here is important: this is not AI as a search engine, or AI as a writing assistant. This is a layperson using AI to navigate a domain that previously required years of graduate training, synthesizing it into a personalized treatment protocol. Whether the vaccine works is almost beside the point — the capability is real and documented, and the implications for democratized medicine, liability, and institutional authority over biological knowledge are profound.

*[@paul_conyngham](https://x.com/paul_conyngham) · Mar 25 · 6.8K views (surfaced by [@DeryaTR_](https://x.com/DeryaTR_) · 2h)*

---

## 9. Vibe Coding's Hidden Cost: Cognitive Atrophy

**Taelin @VictorTaelin · 5h**

Victor Taelin, a developer working on formal verification and type theory, posted a confession that should be read by anyone who has spent serious time with AI coding assistants: "As of March 2026, just prompting agents to implement a termination checker will not work. Even GPT 5.4 Pro's plan is just... bad. Just bad. It seems like I'm gonna need to code this on my own, and my brain is spoiled and lazy from so much vibe coding." Two separate insights are compressed here. First, the hard ceiling: there exist non-trivial software engineering tasks — formal verification, termination analysis — where even frontier models produce bad plans, not just bad code. Second, the cognitive externalization trap: prolonged reliance on AI coding assistance may degrade the practitioner's ability to engage with hard problems independently. This is not technophobia; it's a practitioner reporting atrophy from within the experience.

*[@VictorTaelin](https://x.com/VictorTaelin) · 5h · 18K views, 350 likes*

---

*Compiled by [@bag_of_ideas](https://x.com/bag_of_ideas) · Friday March 27, 2026 · 12-hour window*
