# LinkedIn/Twitter Highlights Post - Friday Noon Edition, April 3 2026

## AI's Compute Plateau Is Reshaping Everything

The most striking signal from today's feed: **Google and Anthropic finished training capable models in March simultaneously**. Not competition. Convergence. According to @AndrewCurran_, this suggests we've hit pure compute saturation—the frontier is no longer about who can run bigger experiments, but who can extract value from what's already been trained.

This inflection point illuminates everything else in today's signal stream.

### **The Gemma Moment**

@fchollet announced Gemma 4 live: four open-weight models under Apache 2.0, with the 31B variant ranking #3 on Arena AI. @demishassabis posted benchmarks showing it beats models 10x its size (log scale). @osanseviero published a visual architecture guide. What matters more than the rankings: @NVIDIA_AI_PC confirmed 2.7x faster inference on RTX with llama.cpp. Translation: open-weight models are no longer research artifacts. They're production assets.

### **The Persistence Layer**

@WesRoth reported Anthropic's Conway—a leaked always-on persistent agent platform running Claude Code 24/7, complete with webhooks, Chrome interface, and CNW ZIP extension standards (essentially an app store for agents). But @maithra_raghu offered a sharp counterpoint: the more capable agents get, the *more* humans we'll need around them—because long-horizon autonomy creates more effort at the handoff points, and the stakes of each autonomous decision rise with capability. The compute ceiling and the autonomy floor are converging, but the human layer isn't going away—it's becoming the critical bottleneck.

### **The Paradigm Collapse**

@emollick declared the RAG era "short-lived but intense"—no longer the dominant paradigm. Long context, tool use, persistent memory are taking over. This isn't hype cycling. It's physics: once models get good enough and inference gets cheap enough, the engineering leverage shifts from retrieval design to orchestration and memory management.

### **The Danger Signal**

But convergence breeds recklessness. @levelsio (of $100K MRR flight sim fame) admitted vibe coding in production is "very dangerous"—literally cutting off database access. @pmarca noted AI increases workload, not reduces it. @garrytan reposted @elvissun arguing "AI slop" is the inevitable future.

And then: @simonw warned of an Axios supply chain attack. North Korean UNC1069 social-engineered a single npm maintainer, compromised a package with 100M+ weekly downloads in 3 hours. Cross-platform RAT shipped. The speed of compromise mirrors the speed of deployment.

### **The Emergence**

Netflix released VOID—their first open-source model that removes video objects *and their physical interactions* from frames. Beijing E-Town's April 19 half marathon will feature 300 humanoid robots from 26 brands running full 21km with 38% autonomous navigation. @rohanpaul_ai covered it.

Meanwhile, 30K LLM agents formalized mathematics. @FabianGloeckle translated an entire grad textbook to Lean. @drfeifei kicked off the 11th year of CS231n.

### **The Unifying Thesis**

We're not in a race for bigger models anymore. We're in a race for *persistent, cheaper, deployable* intelligence at scale. The compute ceiling hit simultaneously for two reasons: (1) scaling laws flatten predictably, and (2) someone finally built tools good enough to extract value from plateau. Gemma's efficiency, Conway's persistence, and the shift away from RAG aren't separate trends—they're the market solving for the same constraint: how do we operationalize frontier capability when scaling compute hits diminishing returns?

The supply chain attack, the vibe coding warnings, the explosion of open models—they're all pressure valves on the same bottleneck.

We've entered the era of *orchestration, not innovation*. And the winners will be whoever can operate fastest at the new ceiling.

Read the full briefing: https://ravi-annaswamy.github.io/dispatches/briefing-2026-04-03-fri-noon/

#AI #GoogleGemma #OpenWeights #AgentArchitecture #ComputeConvergence
