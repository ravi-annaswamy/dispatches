# X/Twitter Briefing — Friday Noon Edition, April 3 2026

**Scanned:** ~20 hours of "Following" timeline | **Captured:** 60+ tweets | **Generated:** Friday April 3, 12:20 PM PT

---

## Gemma 4: Google's Open-Weight Salvo

- **Google DeepMind dropped Gemma 4 in four sizes under Apache 2.0 — and the 31B dense model already ranks #3 among all open models on Arena AI.** François Chollet announced the release live during a Keras community call, calling it the best open-source model for reasoning and agentic workflows. The four sizes (E2B, E4B, 26B MoE, 31B Dense) ship with native function-calling, structured JSON output, and 128K–256K context, with vision and audio coming soon. The Apache 2.0 license is the real story here: no MAU caps, no acceptable-use restrictions, full commercial freedom — Google is betting that openness, not lock-in, wins the developer ecosystem war against Meta's Llama.
  *(François Chollet @fchollet · 12m · 2.6K views)*

- **Demis Hassabis posted a benchmark chart showing Gemma 4 outperforming models over 10x its size — and pointedly noted the x-axis is log scale.** The chart circulated widely after Riley Goodside reposted it. Gemma 4 31B scores 89.2% on AIME 2026 (math), 84.3% on GPQA Diamond (science), and 80.0% on LiveCodeBench v6. These numbers place it in territory previously occupied only by closed frontier models. The upstream enabler: architectural breakthroughs from the Gemini 3 research line, now cascading down to open-weight releases.
  *(Demis Hassabis @demishassabis · 3h · 54K views — the kind of reach that signals a genuine benchmark surprise, not just a press release)*

- **Omar Sanseviero published an architectural deep dive — a visual guide to Gemma 4 covering per-layer embeddings, vision encoders, and audio encoders.** This is the kind of community documentation that accelerates adoption faster than any official blog post. The guide traces the full architecture from input embeddings through the MoE routing to the output heads, with annotations explaining design choices.
  *(Omar Sanseviero @osanseviero · 47m · 5K views)*

- **NVIDIA confirmed Gemma 4 31B runs 2.7x faster on RTX GPUs using llama.cpp — a joint optimization with Georgi Gerganov.** This matters because it means the flagship model is already consumer-GPU-ready on day one. The collaboration between NVIDIA's AI PC team and the llama.cpp maintainer represents the kind of hardware-software co-optimization that used to take months.
  *(NVIDIA AI PC @NVIDIA_AI_PC · 21h · 70K views)*

---

## The Always-On Agent

- **Anthropic is reportedly testing "Conway," an always-on persistent agent platform that transforms Claude from a chatbot into an autonomous digital twin.** The leaked project reveals a dedicated web workspace (not a chat interface) that runs Claude Code continuously, supports external webhooks, interfaces with Chrome, and sends notifications. Most striking: a forthcoming CNW ZIP extension standard that would let developers build custom tools, UI tabs, and context handlers — essentially an app store for persistent AI agents. If Conway ships, it positions Anthropic not as a chatbot company but as an operating-system company.
  *(Wes Roth @WesRoth · 4h · 10K views)*

- **Andrew Curran observed that if OpenAI and Anthropic both finished training "surprisingly capable" large models in early March, the convergence may be purely a result of scale.** This is a sharp inference: two independent labs hitting similar capability thresholds simultaneously suggests the performance is downstream of compute budgets, not unique architectural insights. The implication — capability is becoming a commodity, and differentiation will come from product, deployment, and ecosystem.
  *(Andrew Curran @AndrewCurran_ · 49m · 6.7K views)*

- **Ethan Mollick declared the RAG era "short-lived, but intense" — arguing retrieval-augmented generation is no longer the dominant paradigm for supplying context to agents.** Long context windows, tool use, and persistent memory are displacing the chunked-retrieval approach that defined 2024–2025. RAG isn't dead, Mollick clarifies, but it's been absorbed into a larger toolkit rather than remaining the central organizing principle.
  *(Ethan Mollick @emollick · 1h · 47K views — 47K views on a technical paradigm shift post signals how many practitioners are feeling this transition in their own work)*

- **François Fleuret asked Claude to load a model checkpoint and diagnose performance issues — and called the result "baffling."** The researcher, who's been developing a transformer-diffusion hybrid (Thinkfuser), simply prompted Claude to inspect the weights and flag anything problematic. The strong recommendation suggests Claude found something a human researcher might have missed — a sign that LLMs are becoming genuinely useful as research collaborators, not just code assistants.
  *(François Fleuret @francoisfleuret · 48m · 1.2K views)*

- **Maithra Raghu predicted that more capable AI agents will require more humans around them, not fewer.** Two reasons: long-horizon AI tasks create more human effort at the handoff points, and the stakes of autonomous decisions rise with capability. This runs counter to the replacement narrative but aligns with how organizations are actually deploying agents in practice.
  *(Maithra Raghu @maithra_raghu · 1h · 378 views — low reach but high signal from a respected ML researcher)*

---

## Vibe Coding Meets Reality

- **Pieter Levels admitted that vibe coding in production is "very dangerous" and announced he's cutting off all database access for AI-generated code — running it as a user with almost no permissions.** This from the indie developer who built a flight simulator in three hours with Cursor AI and hit $100K MRR. The upstream cause: a wave of security incidents in early 2026 where AI-coded apps shipped with misconfigured databases, exposed tokens, and overly broad access. Levels' response — sandboxing AI code at the infrastructure level — may become the template for the rest of the vibe-coding community.
  *(Pieter Levels @levelsio · 1h · 85K views — the reach reflects how many developers are having this same reckoning)*

- **Marc Andreessen posted "AI increases workload. Many such cases." — a dry observation that resonated with 109K viewers.** The subtext: AI tools generate so much output so quickly that reviewing, debugging, and integrating it creates net new work. This echoes the growing "AI productivity paradox" literature, where tool adoption increases throughput but also increases the cognitive load of quality control.
  *(Marc Andreessen @pmarca · 8h · 109K views)*

- **Garry Tan reposted Elvis Sun's thread arguing that "AI slop" is actually the future of software engineering — and that mass code review and line-by-line gatekeeping represent legacy thinking.** The FastCompany piece frames the debate as velocity versus craft. The thread drew strong reactions precisely because it challenges the professional identity of developers who prize clean, artisanal code. Whether the future looks more like "AI slop at scale" or "AI-assisted craftsmanship" remains the central culture war in software.
  *(Elvis Sun @elvissun · 17h · 48K views, reposted by Garry Tan @garrytan)*

---

## The Supply Chain Is the Attack Surface

- **Simon Willison warned open-source maintainers that the Axios npm supply chain attack began with "very sophisticated social engineering" targeting a single developer.** The attack, attributed by Google to North Korean group UNC1069, compromised the Axios npm package (100M+ weekly downloads) on March 31. The attackers cloned a legitimate company founder's identity, created a branded Slack workspace, and used it to steal the maintainer's npm credentials. Two trojanized versions (1.14.1 and 0.30.4) shipped a cross-platform RAT that hit macOS, Windows, and Linux systems. The entire window of exposure — from compromise to detection — was roughly three hours.
  *(Simon Willison @simonw · 2h · 7.4K views)*

- **Netflix open-sourced VOID, its first public AI model — a video inpainting system that removes objects along with all the physical interactions they induce on a scene.** Remove a person holding a guitar, and VOID also makes the guitar fall naturally. Built on CogVideoX with a novel "quadmask" conditioning system that encodes primary objects, overlap regions, affected regions, and background. It's trained on paired counterfactual videos from Blender physics simulations. The model is on HuggingFace under an open license. As one commenter noted, more tech companies doing more open source is "the good timeline."
  *(AshutoshShrivastava @ai_for_success · 5h · 2K views; apolinario @multimodalart · 6h · 1.5K views)*

---

## Robots, Proofs & The Physical Frontier

- **Over 300 humanoid robots from 26 brands will compete in Beijing's E-Town Half Marathon on April 19, running the full 21 kilometers alongside human runners.** The event has scaled fivefold from last year: 76 institutions from 13 provinces, 80+ corporate teams, and 20 university teams (10x last year). Robots taller than 75cm must complete the full distance in one continuous effort — no recharging, no resets. Approximately 38% of teams will field robots capable of fully autonomous navigation. A new "Baturu" obstacle challenge on April 18 simulates disaster recovery and industrial scenarios.
  *(Rohan Paul @rohanpaul_ai · 1h · 3.1K views)*

- **Fabian Gloeckle announced a milestone in automatic formalization: translating an entire graduate mathematics textbook into Lean using 30,000 LLM agents.** The open-source project (Blueprint+Lean for algebraic combinatorics) represents large-scale multi-agent inference that actually works in practice. The upstream context: formal verification of mathematics has been a decades-long dream, and the bottleneck has always been the labor of manual formalization. Throwing 30K agents at the problem suggests brute-force scaling may finally be crossing the quality threshold.
  *(Fabian Gloeckle @FabianGloeckle · 2h · 5.5K views, reposted by Gabriel Synnaeve @GabrielSynworker)*

- **Fei-Fei Li kicked off the 11th year of CS231n at Stanford, asking students which departments they come from — and noting that the answer keeps changing.** The original computer vision course has evolved into a cross-disciplinary magnet, drawing students from far beyond CS. This annual ritual is a quiet barometer of how AI education is diffusing across the academy.
  *(Fei-Fei Li @drfeifei · 30m · 2.6K views)*

---

## Culture, Heritage & the Feed's Other Life

- **A heated debate erupted over who best portrayed Lord Rama in Telugu cinema, with PVR Narasimha Rao insisting "NOBODY in Telugu or any other language portrayed Lord Rama and Lord Krishna better than NTR."** The thread, responding to a claim that Harinath Raju and Shobhan Babu surpassed NTR, drew hundreds of views and passionate replies. Rao followed up with a comparison of how NTR played Rama versus Ravana, calling the era one when "writers, directors and actors knew what they were doing." The thread is a reminder that this feed carries a deep cultural memory alongside its AI signal.
  *(PVR Narasimha Rao @homam108 · 3h · 12K views; मङ्गलम् @veejaysai · 9h · 17K views)*

- **A rare six-faced Bhagwan Kartikeya vigraha was discovered in Himachal Pradesh — a find that drew 1,000 likes and 147 retweets from a feed that typically celebrates neural networks, not archaeological ones.** The crossover engagement suggests a community that values heritage as deeply as it values hyperparameters.
  *(Tehxi @yajnshri · 15h · 7.6K views)*

- **Vishal Misra shared a production thread on the Ramayana film, noting that the "obsession and research Nitesh has put in" is visible in ways a 2-minute teaser can't capture.** In a week dominated by AI-generated imagery discourse, a post celebrating years-long human craftsmanship in filmmaking struck a chord.
  *(Vishal Misra @vishalmisra · 6h · 1.2K views)*

---

*A meta-observation: today's feed is bookended by two kinds of craftsmanship — the race to build and deploy AI systems at unprecedented speed (Gemma 4 launching on KerasHub within minutes of the announcement, levelsio shipping to production in hours) and the slow, reverent work of preserving and creating culture (NTR's Rama, a six-faced deity unearthed in the Himalayas, a film decades in the imagining). The tension between velocity and craft is the feed's recurring bass note.*

---

*Compiled by @bag_of_ideas via automated X/Twitter digest*
