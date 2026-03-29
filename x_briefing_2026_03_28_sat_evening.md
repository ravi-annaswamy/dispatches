# X/Twitter Briefing — Saturday Evening Edition, March 28 2026

**Scanned:** ~12 hours of "For you" timeline | **Captured:** 35+ tweets | **Generated:** Saturday March 28, 7:00 PM

---

## AI Models & the Hassabis-Zuckerberg Dinner

- **Demis Hassabis reportedly tested Mark Zuckerberg's reasoning during a private dinner — using the Wason selection task, a classic logic puzzle that most people fail.** Steve Hou surfaced the anecdote from a longer profile: Hassabis steered conversation toward VR, AR, and 3D printing to gauge whether Zuckerberg was thinking about intelligence itself or just chasing the next platform cycle. The subtext is a familiar one in AI leadership circles — Hassabis has always positioned DeepMind as pursuing general intelligence, not just product features, and the dinner reads as a quiet competitive assessment disguised as shop talk.
  *(Liron Shapira @liron · 5h, Steve Hou @stevehou · 8h · 78K views — the anecdote circulated fast, resonating with the growing sense that the Hassabis-Zuckerberg rivalry is becoming the defining one in AI)*

- **Sebastian Mallaby's new book "The Infinity Machine" on Demis Hassabis and DeepMind is drawing early praise as essential reading for understanding the mind shaping AI's direction.** Daniel Rock and Kevin Gee highlighted the book's depth in capturing not just where AI is going but the specific kind of intellect driving it. Mallaby, who wrote the definitive book on venture capital, brings a biographer's rigor to a subject that usually gets hagiographic treatment.
  *(Daniel Rock @danielrock · 12h, Kevin Gee @kevg1412 · Mar 27)*

---

## Claude Code & Developer Tooling Wars

- **Garry Tan revealed he uses /codex adversarial reviews — firing CEO, design, and engineering reviews from GStack — to sharpen his thinking when building with Claude Code as his primary agent.** The trick is using one AI to audit another's output: a meta-layer that catches the assumptions a single-agent workflow misses. This comes as Minh-Phuc Tran noted he's switching from Claude Code to Codex after repeatedly typing "double check if you missed anything," suggesting the tools are converging toward built-in adversarial self-review.
  *(Garry Tan @garrytan · 12h · 17K views)*

- **Developers are frustrated by Claude Code's tightened rate limits, with 267 posts trending on the topic in the last 2 hours.** The rate limit squeeze is forcing power users to optimize their workflows — which is exactly what aditya's viral article addresses, arguing most people waste 70% of their Claude budget by treating it like a faster ChatGPT instead of structuring prompts for efficiency.
  *(Trending · 2h · 267 posts; aditya @adxtyahq · 10h)*

- **MIT CSAIL shared a "Build Any App: The Technical Co-Founder" mega-prompt for Claude — a five-phase framework (Discovery, Planning, Building, Polish, Handoff) that treats the AI as a co-founder rather than a code generator.** The prompt, by Miles Deutscher, includes instructions that sound more like a co-founder agreement than an engineering spec. The key insight: it tells Claude to challenge assumptions and separate "must have now" from "add later" — the kind of product discipline that usually requires a human partner to enforce.
  *(MIT CSAIL @MIT_CSAIL · 12h · 42K views)*

- **Kevin Simback asked the question every Claude Code team is now debating: gstack (Garry Tan's adversarial review system) or Compound Engineering (by Every) — and concluded the answer is both.** The emerging pattern is layered tooling: Claude Code for generation, gstack for review, Compound Engineering for orchestration. The Claude Code ecosystem is fragmenting into specialized roles faster than anyone expected.
  *(Kevin Simback @KSimback · Mar 27, reposted by Garry Tan · 44K views)*

- **Ishan teased something useful for Claude Max plan subscribers, drawing 110 likes and 13K views with zero details.** The Claude Max plan — Anthropic's premium tier — is becoming a status signal in developer circles, with an ecosystem of tools and tips building around the cohort of users willing to pay top dollar for AI access.
  *(Ishan @radshaan · 4h · 13K views)*

---

## AI Infrastructure & Performance

- **A single developer rewrote vLLM in Rust (calling it rvLLM), spent 22 hours and $1,780, and hit 10,291 tokens/second — beating Python vLLM up to N=256 with 20x faster startup.** The article claims 31x improvements on some operations. The upstream enabler is Rust's zero-cost abstractions meeting LLM inference's embarrassingly parallel workload. If a weekend project can outperform the standard Python inference stack, it raises uncomfortable questions about the technical debt baked into the current AI infrastructure.
  *(andy @1a1n1d1y · 18h · 74K views — strong engagement for a deep-systems post)*

- **Prince Canuma announced mlx-vlm v0.4.2 with Meta's SAM3 model — adding realtime mask-only label drawing to Apple Silicon.** The MLX ecosystem for on-device AI continues to mature quietly. SAM3 running locally on a MacBook is the kind of capability that was cloud-only six months ago.
  *(Prince Canuma @Prince_Canuma · 7h · 56K views)*

---

## AI Research & Intelligence Theory

- **Jonathan Ross argued that the scaling laws paper is the most misread paper in AI — people see "exponential compute for linear improvement" and conclude AI is slowing down, but they're missing something.** The post drew 460 likes and 82K views, suggesting the "AI is hitting a wall" narrative has enough believers that a counter-argument resonates. The scaling debate is becoming the field's central fault line.
  *(Jonathan Ross @JonathanRoss321 · 14h · 82K views)*

- **Karpathy's AI persuasion experiment hit trending with 4,367 posts — exposing how effectively LLMs can shift human opinions.** The experiment apparently demonstrated that LLMs can be more persuasive than humans in structured argumentation, raising questions about AI's role in shaping belief at scale. This sits at the intersection of capability research and governance that rarely gets this kind of viral attention.
  *(Trending · 9h · 4,367 posts)*

- **Josh proposed a hypothesis that could reshape AI evaluation: for every unverifiable task, there exists a set of related verifiable tasks where hillclimbing generalizes to the original.** Brendan Dolan-Gavitt prompted this with "there are verifiable rewards everywhere for those with eyes to see." If Josh's hypothesis holds, it means the "alignment is impossible because we can't verify the important things" argument may have a workaround — train on verifiable proxies that transfer.
  *(Josh @JoshPurtelL · 4h · 3.7K views; Brendan Dolan-Gavitt @moyix · 6h)*

- **Haider predicted ARC-AGI 4 could be solved sooner than expected — if agents achieve superhuman logical deduction on ARC 3, the skills transfer directly since ARC 4 follows clear logical rules rather than subjective preferences.** The ARC benchmark remains François Chollet's signature contribution to the AI evaluation space, and Chollet himself was trending today arguing that intelligence resembles something the feed didn't fully reveal.
  *(Haider @slow_developer · 3h · 2.5K views)*

- **An arxiv paper on "Arrows of Time for Large Language Models" circulated, studying whether autoregressive LLMs exhibit a temporal directionality bias in their probabilistic modeling.** The question is subtle but fundamental: do LLMs reason about the past and future symmetrically, or do they inherit a directional arrow of time from their training data? The paper drew 195 likes from a technical audience, suggesting it touches a genuine open question.
  *(arxiv · 195 likes · 9.3K views)*

---

## The Alec Radford Appreciation Thread

- **A viral thread positioned Alec Radford — the researcher who built GPT-1 when no one else at OpenAI believed in pretraining transformer language models — as the single most important and least famous figure in AI.** Joseph Francis kicked it off sarcastically ("None of this guy's stuff has been peer reviewed. Loser.") while showing Radford's Google Scholar page: 68,880 citations for GPT-3, 57,679 for CLIP. Flowers followed up noting that every LLM from every lab traces back to Radford's lonely bet on pretraining. The thread is a reminder that the most consequential research decisions often look like career suicide at the time.
  *(joseph francis @joefrancis505 · 11h; Flowers @flowersslop · 14h · 258K views combined)*

---

## AI Creative Tools & Filmmaking

- **Viktor Oddy combined NanoBanana + Kling 3 + Claude to build "Aethera" — a landing page so polished it drew 1.3K likes and 107K views.** The stack is becoming a standard creative pipeline: AI image generation (NanoBanana), AI video (Kling), and AI orchestration (Claude). What took a design agency a week now takes a solo creator an afternoon.
  *(Viktor Oddy @viktoroddy · 13h · 107K views)*

- **Paige Bailey showcased NanoBanana use cases from UCLA's Glitch Hacks hackathon — including decomposing images into step-by-step drawing tutorials using Google AI Studio.** The hackathon application turns complex images into beginner-friendly drawing guides, which is a clever inversion: using AI not to create art but to teach the process of creating art.
  *(Paige Bailey @DynamicWebPaige · 23h · 12K views)*

- **An AI film studio claimed to be making films for governments and billion-dollar companies, with a complete guide to Seedance 2.0 drawing 1K likes and 201K views.** EP separately noted that the deals people are making in AI filmmaking are reaching a scale that surprised even insiders. The AI filmmaking space is crossing from hobby to industry faster than AI art did.
  *(EP @eptwts · 12h · 81K views; Seedance 2.0 article · 201K views)*

- **Levelsio made his code-generated designs interactive — turning every AI idea into a launchable app — then asked the logical next question: why not auto-generate every idea, add Stripe, and launch automatically?** The comment about AI designs all converging on brown tones and serif fonts when asked to avoid cliche is a small but revealing observation about AI's aesthetic blind spots.
  *(levelsio @levelsio · 1h–6h · 19K views)*

---

## Geopolitics: The Iran Crisis

- **A crypto analyst connected dots that nobody else was drawing: Iran mines Bitcoin at $1,300 per coin, sells every coin at market price the same day. The US bombed their power grid for 27 days. BTC pumped from $71K to $74K in the same window. Then Trump paused strikes — and Iran's mining machines came back online.** The thread claims the BTC sell pressure resumed as Iran's grid recovered, drawing 1.8K likes and 811K views. Whether the causal chain holds or not, the tweet frames the Iran conflict through a lens that traditional geopolitical analysis ignores entirely.
  *(cape @capexbt · 11h · 811K views — the most-viewed non-entertainment tweet in this scroll)*

- **Rajdeep Sardesai reported that Elon Musk joined the PM Modi-Trump phone call amid the Iran conflict (per NYT), raising questions about what a private citizen was doing on a wartime call between heads of state.** The Modi-Trump call itself is significant — India has been walking a diplomatic tightrope on Iran — but Musk's presence is the detail that makes it extraordinary.
  *(Rajdeep Sardesai @sardesairajdeep · Mar 28 · 34K views)*

- **India went into full security mode: Modi met all state Chief Ministers, Ajit Doval conducted a high-level security meeting, and Rajnath Singh met with other ministers.** The thread by Berlin drew 7.2K likes and 472K views, indicating the India-focused audience is watching the Iran escalation with intense concern. A Gulf diplomat told Okonkwo that the strategic picture is bigger than anyone is seeing, with Israel's bombing of Iran's gas fields part of a broader realignment.
  *(Berlin @Toxicity_______ · 17h · 472K views; Okonkwo @EmekaCryptoNG · 8h)*

---

## Indian Heritage & History

- **Gaurav Sabnis shared a remarkable cross-cultural story: a cabbie in Mexico recognized "Nagpur" and pointed him to a Diego Rivera mural featuring Dr. Pandurang Sadashiv Khankhoje — a Nagpur-born agronomist who became Mexico's "Norman Borlaug of corn."** The mural, in Mexico's Education Secretariat, is a physical record of an Indo-Mexican scientific exchange that most Indians have never heard of.
  *(Gaurav Sabnis @gauravsabnis · 12h)*

- **Varsha Singh posted a video of an 1800-year-old Devi Mahatmya scripture from Oxford University, drawing 5.9K likes and 62K views.** The artifact connects to the broader question of how Indian manuscripts ended up in European university collections — a topic that reliably generates both awe and indignation on Indian Twitter.
  *(Varsha Singh @varshaparmar06 · 16h · 62K views)*

---

## Quotable & Resonant

- **Nokia collects a hidden royalty on every smartphone sold — owning 20K+ patent families covering the foundational math for 4G, 5G, and the upcoming 6G.** Parimal's thread drew a staggering 2.1 million views, turning an obscure fact about patent licensing into viral content. Nokia's quiet transformation from phone maker to patent licensor is one of the most underreported business stories in tech.
  *(Parimal @Fintech03 · 21h · 2.1M views)*

- **Alex Kontorovich highlighted a hierarchy of success: Speak > Write > Have good ideas — in that order — citing MIT professor Patrick Winston's legendary 18-million-view "How to Speak" lecture.** The implication is uncomfortable for researchers and builders: the quality of your ideas matters less than your ability to communicate them. Winston's lecture, delivered in 2019, continues to circulate because the insight never stops being relevant.
  *(Alex Kontorovich @AlexKontorovich · 9h)*

- **Vinod Khosla argued that the biggest risk right now is not taking risks — quoting a CEO letter (via Alfred Lin) about leading through compounding change.** The post drew 478 likes and 149K views, suggesting the VC class is bracing for a period where conservative strategies become the most dangerous ones.
  *(Vinod Khosla @vkhosla · 9h, reposted by Malaikannan Sankarasubbu · 149K views)*

- **Bret Weinstein drew an unexpected parallel between prompting LLMs and prompting students: "Answer the question I should have asked you rather than the one I did ask you."** The Wyndo prompt he was quoting — "Interview me until you have 95% confidence about what I actually want, not what I think I should want" — captures the gap between stated and actual requirements that kills most projects.
  *(Bret Weinstein @BretWeinstein · 5h)*

---

*A feed shaped by two gravitational forces tonight: the Iran crisis pulling in geopolitical anxiety, and Claude Code's ecosystem pulling in builder energy. The Alec Radford thread is the quiet highlight — a reminder that the most important bets in AI were made by people whose names most people still don't know. Project Hail Mary, meanwhile, sits there with 4.8 million views, evidence that this audience still looks up.*

---

*Compiled by @ravi_annaswamy via automated X/Twitter digest*
