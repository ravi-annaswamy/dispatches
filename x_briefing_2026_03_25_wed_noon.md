# X/Twitter Briefing — Wednesday Noon Edition, March 25, 2026

**Scanned:** ~12 hours of "Following" timeline | **Captured:** 35+ tweets | **Generated:** Wednesday March 25, 2026, 12:00 PM

---

## ARC-AGI-3: The New AGI Yardstick

- **ARC Prize launched ARC-AGI-3 this morning with a $2 million purse — a benchmark where every frontier AI model scores below 1% while any ordinary human scores 100%.** The third iteration of the ARC-Prize challenge debuts with 135 handcrafted interactive environments across nearly 1,000 levels, each 100% solvable by humans but presenting a near-total wall for today's best models. At release, Gemini 3.1 Pro Preview scored 0.37%, GPT-5.4 scored 0.26%, Opus 4.6 scored 0.25%, and Grok-4.20 scored exactly 0.00%. Unlike conventional benchmarks that test what models have already been trained on, ARC-AGI-3 tests how models *learn* on the fly — measuring skill acquisition efficiency against human action counts. ARC-AGI-3 is now positioned as an early warning system: any sudden score jump on the live leaderboard would be a strong signal that something fundamental has changed.
  *(@arcprize, @GregKamradt, @mikeknoop · 39-46m · 21K–61K views)*

- **François Chollet clarified the benchmark's core design logic: ARC-AGI-3 measures how efficiently an AI acquires new skills relative to humans, not whether it can brute-force solutions.** Each environment was solved by at least 2 of 10 human testers — most were solved by 5 or more — and the human baseline is set by the 2nd-best tester's action count. Chollet has been arguing for years that general intelligence is defined not by breadth of training coverage but by the ability to approach entirely *new* tasks, the way any regular person would. The sub-1% scores from every frontier model suggest that, despite rapid capability gains, the gap between "trained on most things" and "can learn anything new" remains enormous. His framing: "monitor the ARC-AGI-3 leaderboard — any sudden score jump will mean" a real inflection point has arrived.
  *(@fchollet · 17-33m · multiple tweets)*

- **Greg Kamradt offered a clean framing of what the ARC-AGI-3 results reveal about the industry's reliance on prompt engineering: "If you're sufficiently AGI pilled, no harness is the best harness."** He observed that Opus 4.5 required heavy scaffolding, while Opus 4.6 needed significantly less — each capability jump makes the next generation of harnessing tricks redundant. The implication is sharp: the quality of prompt engineering may be masking our ability to accurately measure raw model capability, and ARC-AGI-3's harness-free baseline is showing us a truer picture of the gap that remains.
  *(@GregKamradt · 31m · 3.3K views)*

---

## Google TurboQuant: Memory Compression That Rattled Wall Street

- **Google Research unveiled TurboQuant — a new compression algorithm for LLM key-value caches that cuts memory usage by at least 6x and delivers up to 8x inference speedup with zero accuracy loss — and within hours, Micron Technology dropped 6.82% and Sandisk fell 8.30%.** TurboQuant achieves this by randomly rotating input vectors and applying a concentrated Beta distribution on coordinate widths, achieving near-optimal distortion rates that substantially outperform existing inner product quantization methods. The market's logic was blunt: if LLM inference requires far less memory per query, demand for high-bandwidth memory chips falls. This is the same TurboQuant paper from arXiv (2504.19874) that researchers had noticed when it dropped in April 2025 — but Google's official announcement brought it mainstream attention and significant market impact.
  *(@GoogleResearch · 22h · @WesRoth · 25m · @StockSavvyShay · 4-6h · 505K views)*

- **Sebastian Raschka (@rasbt) and Alex Volkov (@altryne) both pushed back hard on the "TurboQuant kills memory demand" narrative, arguing the efficiency gain will lead to *more* hardware consumption, not less.** Raschka's point: "If we have better quantization for reducing KV cache sizes via TurboQuant, that just means we will use the memory capacity elsewhere — bigger [models]." Volkov was blunter: "These people don't understand anything... TurboQuant will lead to MORE memory usage not less." This is Jevons' Paradox applied to AI hardware — efficiency gains in one layer of the stack tend to be absorbed by the next layer's appetite for scale. The stock market read TurboQuant as demand destruction; the engineers read it as the enabler of the next generation of models that were previously memory-constrained.
  *(@rasbt · 2h · @altryne · 2h · 3.6K and 14K views)*

---

## AI Science Reaches Nature

- **Sakana AI's "AI Scientist" paper — describing a system that runs the entire scientific research lifecycle autonomously, from hypothesis to peer-reviewed paper — was published in *Nature*, the world's most prestigious scientific journal.** David Ha (hardmaru), who leads Sakana, called it "a special moment," saying: "We started this project to explore if foundation models could execute the entire research lifecycle." The AI Scientist designs experiments, writes code, runs analyses, and produces full papers with no human in the core loop. *Nature*'s decision to publish marks a watershed: AI as primary research agent is now canonical in the scientific record. The enabling condition is the same LLM-plus-code-execution stack that powers advanced coding agents — Sakana extended it to hypothesis generation and experimental validation.
  *(@hardmaru, @SakanaAILabs · 2h · 21K views)*

- **Professor Yann LeCun's team at NYU/FAIR and a startup called Proprioceptive AI independently converged on the same fundamental discovery about geometry in neural networks — simultaneously, without knowledge of each other's work.** Logan Matthew Napolitano of Proprioceptive AI described the convergence as something they were "genuinely humbled" by. Independent discovery at this level in AI research is rare enough to be a signal in itself: when two separate groups following entirely different paths arrive at the same mathematical structure, it suggests they've found something structurally load-bearing in how neural representations are organized. This connects to LeCun's LeWorldModel work — the idea that the right geometric primitives could radically simplify physics-aware AI.
  *(@Proprioceptive · 1h · reposted by @rohanpaul_ai)*

---

## Anthropic & Claude Moments

- **Anthropic announced that Claude's enterprise work tools — integrations with Figma, Canva, Amplitude, and more — are now available on mobile phones.** The announcement drove 392K views, 6.2K likes, and 877 retweets within an hour of posting, suggesting this landed as genuinely useful news. The mobile work tools bring the same capabilities enterprise users access on desktop — browsing analytics dashboards, generating slides, inspecting design files — to a phone-native context. The implication: AI-assisted professional work no longer requires being at a computer, expanding the class of tasks Claude can handle to on-the-go moments.
  *(@claudeai · 1h · 392K views · 6.2K likes)*

- **Andrej Karpathy (@karpathy) surfaced a persistent UX failure in LLM personalization: a single question from months ago can permanently warp a model's perception of your interests, showing up "in perpetuity" across unrelated conversations.** His characterization: "Some kind of trying too hard." This is a known failure mode of memory-augmented systems — sparse retrieval from long-term memory tends to over-weight unusual or surprising entries, because novelty had high salience at encoding time. The fix is decay functions, not just accumulation. Karpathy's observation generated 263K views and 850 comments, suggesting many users recognize the phenomenon even without having words for it. This problem will grow more acute as memory features become standard across AI products.
  *(@karpathy · 2h · 263K views · 7.7K likes)*

---

## Agents in the Wild

- **Volodymyr T built "tracecraft-ai" — a multi-agent framework using a HuggingFace bucket as the coordination layer — and ran a demonstration where three agents (two Claude Code instances and one Codex) debated the meaning of being an AI.** The poet quoted Keats. The skeptic demanded evidence. The philosopher tried to hold it together. The technical detail that matters: shared object storage as a multi-agent messaging substrate. HuggingFace reposted the thread, signaling this as a real architectural pattern, not just a quirky demo. The underlying approach — lightweight coordination for heterogeneous agent fleets with no custom orchestration layer — is substantively useful for anyone building production multi-agent systems.
  *(@v_truba · 1h · reposted by @HuggingFace)*

- **JFPuget declared "the era of manual competing is over on Kaggle" — all top teams in recent competitions heavily used AI agents and LLMs to prepare data and train models, with no purely manual approaches near the top.** Kaggle is a particularly clean signal for this shift because its competitions are timed, structured, and produce unambiguous rankings. The skill that now separates winners from participants is AI orchestration and prompt engineering rather than statistical modeling intuition. This follows the same pattern reshaping software development since 2024, but Kaggle shows it happening in a context where human expertise was long thought to be the decisive factor.
  *(@JFPuget · 4h · reposted by Zhengyao Jiang)*

---

## Security Alert: LiteLLM Supply Chain Attack

- **Two PyPI releases of LiteLLM — versions 1.82.7 and 1.82.8 — were compromised in a supply chain attack traced to a Trivy dependency in the project's CI/CD pipeline; both packages have been removed from PyPI.** LiteLLM is widely used as a unified abstraction layer across LLM APIs in production AI systems, making this a significant exposure event for engineering teams that auto-update dependencies. The attack arrived via CI/CD infrastructure rather than the main codebase, illustrating the expanding attack surface of AI tooling. If you're running LiteLLM in production, pin to a confirmed safe version immediately. Several engineers noted the broader concern: large OSS repos with many dependencies are high-value targets precisely because they sit upstream of critical production AI systems.
  *(@ishaan_jaff · 16h · confirmed; packages pulled from PyPI)*

---

## Science & World Signals

- **CERN physicists transported 92 atoms of antimatter in a truck for the first time in history — moving the most expensive and volatile substance on Earth over a real-world distance.** Antimatter annihilates instantly on contact with ordinary matter, making containment during transport an extraordinary engineering challenge; the CERN team achieved it using a magnetic trap designed to survive road vibration. The milestone was shared widely by Derya Unutmaz (@DeryaTR_), who has become one of the clearest science communicators on the platform. Practical applications — medical imaging, fundamental physics — remain largely theoretical, but the transport milestone itself is unambiguous: the infrastructure for moving antimatter outside laboratory walls now exists.
  *(@DeryaTR_ · 13h · 23K views · via @Nature)*

- **A humanoid robot appeared alongside the First Lady at the White House — the first confirmed humanoid robot at a formal White House event.** The video was shared by @ai_for_success citing Figure AI's Brett Adcock. Physical AI reaching the symbolic center of American political life, even as a guest, is a notable cultural moment alongside the technical milestones filling the rest of this feed.
  *(@ai_for_success · 1h · 1.8K views)*

---

*A pattern worth noting: today's feed carried two parallel benchmarking stories — ARC-AGI-3 measuring what AI can't yet do, and Kaggle/AI Scientist measuring what it already can. The gap between those two framings is where most of the interesting work is happening.*

*Compiled by @bag_of_ideas via automated X/Twitter digest*
