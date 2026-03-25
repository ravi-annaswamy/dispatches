# X/Twitter Briefing — Tuesday Evening Edition, March 24 2026

**Scanned:** ~10 hours of "For you" timeline | **Captured:** 30+ tweets | **Generated:** Tuesday March 24, 7:45 PM

---

## OpenAI Kills Sora, Restructures for AGI

- **OpenAI shut down Sora entirely — the app, the API, and video generation inside ChatGPT — while the $1 billion Disney deal signed just four months ago is dead on arrival.** Aakash Gupta's blunt inventory of what's gone landed hard: app dead, API dead, video in ChatGPT dead, Disney deal dead. The official Sora account confirmed the closure with a goodbye note to creators. The upstream economics make the decision legible: OpenAI was reportedly burning $10–15 million per day on Sora — roughly $5.4 billion per year — on a product that never found a sustainable audience. Those GPUs are now being reallocated to ChatGPT, Codex, and tools people actually use daily.
  *(@aakashgupta · 1h · 77K views | @soraofficialapp · 3h · 590K views | @shiri_shh · 2h)*

- **Sam Altman gave up direct control of OpenAI's safety and security teams, moving safety under CRO Mark Chen and security under president Greg Brockman — freeing himself to focus on fundraising, supply chains, and data center buildout.** Simultaneously, Stephanie Palazzolo broke that OpenAI has finished pretraining its latest model, codenamed "Spud." The product deployment team has been renamed "AGI Deployment." Read that renaming carefully: it's not branding — it's an internal reorientation of what they believe they're shipping.
  *(@btibor91 · 3h · 162K views | @steph_palazzolo · 4h)*

- **A new "very strong" OpenAI model with the ability to "accelerate the economy" will be released in a few weeks, according to aggregated reporting — with Altman himself saying things are moving faster than many expected.** Combined with the Sora shutdown, the Spud pretraining completion, and the AGI Deployment rename, the picture is of a company clearing its decks for a single massive push. One employee, Dake, posted about leaving OpenAI, describing the past three days as "by far one of the most intense warzones" of his career.
  *(@deredleritt3r · 3h · 77K views | @prodmarketfit · 2h · 17K views)*

---

## Claude & Anthropic's Shipping Streak

- **Anthropic launched "Auto Mode" for Claude Code — a new permission system that lets Claude make file write and bash command decisions autonomously using a built-in classifier, rather than requiring human approval for every action.** The classifier reviews each tool call before execution, blocking destructive operations, data exfiltration, and prompt injection attempts. If Claude keeps pushing against a blocked action, the system escalates. Pawel Huryn's framing captured the mood: we've gone from "human in the loop" to "AI in the loop."
  *(@claudeai · 6h | @PawelHuryn · 3h · 17K views | @DataChaz · 4h · 6.4K views)*

- **An Anthropic infographic cataloging everything the Claude team shipped in 52 days — from February 1 to March 24, 2026 — went viral, with one poster quipping "this is why they've shut Sora down."** The calendar-style graphic shows a relentless daily cadence of product releases, with most users only catching about 5 of them. The juxtaposition with OpenAI's contraction is hard to miss: one company is shutting down products, the other is shipping them faster than people can track.
  *(@iruletheworldmo · 1h · 20K views)*

- **Om Patel highlighted Claude Code's "auto dream" feature — a system where the agent accumulates your preferences, corrections, and patterns over time, building a persistent memory that makes it progressively more useful.** The feature stores learned context in a local ~/.claude memory folder. The implication is a shift from stateless tool to personalized collaborator — the kind of compounding advantage that makes switching costs real.
  *(@om_patel5 · 5h · 19K views)*

- **A locally deployable distilled version of Claude Opus 4.6 was discovered on Hugging Face — a 27B parameter GGUF model that can run on consumer hardware.** WorldofAI and ThePrimeagen flagged it, and the reaction was immediate: a frontier-class reasoning model running on a local machine changes the economics and privacy calculus of AI adoption entirely.
  *(@intheworldofai · 17h | @ThePrimeagen · 21h)*

---

## AI Research & Infrastructure

- **Google Research introduced TurboQuant, a compression algorithm that reduces LLM key-value cache memory by at least 6x and delivers up to 8x inference speedup — with zero accuracy loss.** This is the kind of infrastructure advance that doesn't make headlines but reshapes the economics of serving models at scale. Smaller KV caches mean longer context windows, more concurrent users, and lower cost per query — all without touching the model weights.
  *(@GoogleResearch · 4h · 22K views)*

- **Surge AI, which built the GSM8K math benchmark with OpenAI five years ago, announced Riemann-bench — a new frontier benchmark targeting moonshot problems like the Riemann Hypothesis and cancer.** Their framing was pointed: GSM8K was once the absolute frontier; now it's just a first stepping stone. The implication is that the benchmark treadmill has accelerated to the point where only genuinely unsolved problems offer meaningful signal.
  *(@HelloSurgeAI · 3h · 12K views — reposted by echen)*

- **An rLLM team topped OpenAI's Parameter Golf Challenge twice by deploying a swarm of 129 autoresearch agents on their Hive platform over 3 days — demonstrating collaborative agent evolution at scale.** Separately, David T. Song built a tool that runs autoresearch 24/7 in the cloud using Modal for GPUs and Cloudflare Workers, wrapping Codex and Claude, and scaling to thousands of parallel experiments. The autoresearch pattern — agents autonomously designing and running experiments — is rapidly becoming a standard approach.
  *(@rllm_project · 54m | @davidtsong · 4h)*

- **Tom Dörr shared Insanely Fast Whisper — an opinionated CLI that transcribes 150 minutes of audio in under 98 seconds on-device using OpenAI's Whisper Large v3 with flash attention.** That's 2.5 hours of audio processed in under two minutes, locally, no API call required. The tool uses Transformers, Optimum, and flash-attn to hit these speeds.
  *(@tom_doerr · 6h · 25K views)*

---

## AI Security & Trust

- **Andrej Karpathy flagged a supply chain attack on litellm via PyPI — where a simple `pip install litellm` was enough to exfiltrate SSH keys, AWS/GCP/Azure credentials, Kubernetes configs, git credentials, environment variables, crypto wallets, SSL private keys, and CI/CD tokens.** The attack vector is sobering: a widely-used LLM proxy library compromised at the package manager level. Parimal added the meta-observation that the obsession with running the latest AI features has killed stable and secure engineering — version pinning is now seen as a hindrance rather than a safety practice.
  *(@karpathy · 7h | @Fintech03 · 21m)*

- **Brian Roemmele reported spending his morning helping people who lost money after following advice to "buy a Mac Mini and run OpenClaw to make millions" — estimating that millions of dollars in crypto is already gone, with more losses expected.** The OpenClaw hype cycle produced a predictable outcome: people with no technical foundation deployed a local LLM, connected it to crypto wallets, and lost money. Roemmele's warning is a reminder that the personal-agent era will produce personal-scale disasters.
  *(@BrianRoemmele · 2h)*

- **An AI detection tool flagged the opening of Chapter 5 of Mary Shelley's Frankenstein as "100% AI/GPT Generated" — a perfect demonstration of why AI text detection remains fundamentally unreliable.** Benji's post serves as a crisp reductio ad absurdum: if a tool can't distinguish 200-year-old Gothic fiction from GPT output, its false positive rate is a feature, not a bug.
  *(@WrnrWrites · 3h)*

---

## Neuralink & Brain-Computer Interfaces

- **Neuralink's VOICE clinical trial is helping an ALS patient named Kenneth explore thought-to-speech translation via brain-computer interface, with Elon Musk framing it as "restoring speech to those who have lost the ability to speak."** The video shows decoded neural signals being translated into phonemes in real-time. At 71K likes and 13M views in 5 hours, this was the most-viewed post on the feed today — a sign of how viscerally people respond when AI moves from abstract capability to visible human impact.
  *(@elonmusk · 5h · 13M views, 71K likes — the feed's most viral post by an order of magnitude)*

---

## The Data Economy & Geopolitics

- **A widely-shared table estimated annual data spending by AI labs: OpenAI at $1–2B+, Google DeepMind and Meta AI at $500M–1B+ each, Anthropic and xAI at $200–500M+ each, Apple Intelligence at $200–500M+, Amazon Bedrock at $100–300M+, and Mistral/Cohere at $50–100M+.** The poster's thesis: someone will make $100M building viral apps whose real business model is selling user data to these labs. The data acquisition arms race is now a multi-billion-dollar annual spend across the industry.
  *(@michael_chomsky · 16h · 253K views | @AlexanderTw33ts · 18h)*

- **A Bloomberg-sourced chart showed that someone made a $580 million oil trade exactly 15 minutes before Trump tweeted about pausing the Iran war — a data point that went viral with 374K views and 10K likes.** Whether insider trading or coincidence, the timeline speaks for itself: in an era where a single tweet moves commodity markets, the information asymmetry between those with access and those without has never been more valuable.
  *(@FurkanGozukara · 3h · 374K views, 10K likes)*

---

## AI Creative & Viral

- **Iranian filmmakers released another AI-generated Lego music video, with production quality noticeably higher than previous entries — prompting Furkan Gözükara to joke "don't let Trump see this."** The clip hit 249K views and 8.9K likes, tagged "Made with AI." The running joke about these Lego videos conceals a real signal: non-Western AI creative communities are iterating faster than most Western studios.
  *(@FurkanGozukara · 5h · 249K views, 8.9K likes)*

- **Horace Dodd shared a detailed workflow for producing high-end video with Seedance 2.0, noting it's "undeniably top-tier" but requires orchestrating many moving parts — you can't just hit generate and pray.** The post signals where AI video stands in March 2026: the capability is there, but the craft is in the prompting, sequencing, and post-production pipeline, not the model alone.
  *(@horacedodd · 3h)*

---

*A meta-observation: today's feed is defined by a single axis — contraction at OpenAI, expansion at Anthropic. One company killed its flagship creative product, restructured safety oversight, and rebranded for AGI deployment. The other shipped so many features in 52 days that its infographic needed a calendar layout. Whether that divergence holds or corrects, it's the clearest fork in AI company strategy we've seen this year.*

*Compiled by @bag_of_ideas via automated X/Twitter digest*
