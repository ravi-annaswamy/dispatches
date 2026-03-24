# X/Twitter Briefing — Monday Evening Edition, March 23 2026

**Scanned:** ~12 hours of "For you" timeline | **Captured:** 30+ tweets | **Generated:** Monday March 23, 7:30 PM

---

## Claude & Anthropic Ecosystem

- **Anthropic launched Claude's computer use for Mac — enabling Claude to physically point, click, scroll, and navigate across any app on a user's desktop.** The feature, announced today via @claudeai, lets Claude operate a user's machine the way a human sitting at a desk would: opening apps, filling spreadsheets, navigating browsers. With 2.8K likes and 278K views in four hours, the reaction is immediate and intense — this is Anthropic's clearest move yet toward making Claude a persistent desktop co-worker rather than a chatbot in a tab. "Claude Cowork" was trending in Technology at the time of this scan.
  *(Claude @claudeai · 4h · 278K views, 2.8K likes — trending in Technology)*

- **Anthropic introduced its Science Blog, positioning scientific acceleration as a core part of the company's mission alongside safety.** The blog will feature new research and stories of how scientists are using AI to accelerate their work. The upstream signal here is strategic: Anthropic is diversifying its public identity beyond safety research toward being seen as a platform for scientific discovery, mirroring Dario Amassei's earlier essay on the intelligence explosion's benefits.
  *(Anthropic @AnthropicAI · 5h · 129K views, 2.4K likes)*

- **Ethan Mollick observed a sharp philosophical split between OpenAI's Codex and Claude Code skills — Codex skills are functional technical references, while Claude skills teach the AI approaches to problems.** The distinction is revealing: OpenAI's skills tell the model what to do; Anthropic's skills tell it how to think. This difference in philosophy maps neatly onto each company's broader identity — one engineering-first, the other more interpretive and adaptive.
  *(Ethan Mollick @emollick · Mar 22 · 69K views, 810 likes)*

- **Wes Roth reported that Anthropic is quietly building a dedicated Projects layer for Claude Cowork on the desktop app, with local folders and project-specific scheduling.** This was independently confirmed by TestingCatalog News. The move extends Claude Cowork from a per-session tool into a persistent project management surface — the kind of feature that turns occasional use into daily habit.
  *(Wes Roth @WesRoth · Mar 20 · reposted today)*

- **Sahil Lavingia, Gumroad founder, turned his book The Minimalist Entrepreneur into 9 Claude Code skills — from /find-community to /marketing-plan — essentially encoding an entire business philosophy into executable AI workflows.** The move is a proof-of-concept for a new form factor: books as code. Rather than reading a chapter on pricing, you invoke /pricing and get an interactive analysis adapted to your specific product.
  *(Sahil Lavingia @shl · 6h · 50K views, 951 likes)*

---

## AI Agents & Self-Improvement

- **Jeff Clune's team released HyperAgents — a self-improving AI system that extends the Darwin Gödel Machine by improving not just its task performance but the very mechanism by which it improves.** Co-authored by Jenny Zhang and colleagues across UBC, Vector Institute, Edinburgh, NYU, and Meta, HyperAgents introduces "self-referential agents" that integrate a task agent and a meta-agent into a single editable program. The key breakthrough: by making the improvement procedure itself editable, the system breaks the assumption that task performance and self-modification skill must be aligned — enabling open-ended self-acceleration across coding, paper review, robotics reward design, and Olympiad math.
  *(Jeff Clune @jeffclune · 9h · Jenny Zhang @jennyzhangzt · 10h)*

- **Mckay Wrigley, who in December declared "you're like 6 prompts away from infinitely customizable personal AGI," is now privately testing a new tool aimed at Claude Cowork, OpenClaw, and Manus users.** The 4-hour self-destruct timer on his DM call suggests a deliberate scarcity play, but the underlying signal is real: the personal-agent tooling layer is getting crowded fast.
  *(Mckay Wrigley @mckaywrigley · 1h · 23K views)*

- **Someone posted a photo of a Mac mini farm — racks of Apple silicon boxes — captioned with the observation that you can run OpenClaw AI agents on these all day long, "or it may be just bot farm."** The ambiguity is the point: the hardware cost of running persistent AI agents has collapsed to the point where a shelf of Mac minis in someone's apartment becomes a plausible agentic computing cluster.
  *(From Rakesh B · 52K views, 339 likes)*

---

## Jensen Huang & the AGI Moment

- **Jensen Huang told Lex Fridman "I think we've achieved AGI" — the most direct claim of its kind from a major industry leader, made on the most prominent AI interview platform.** Lex's framing was characteristically maximalist: the definition he offered was an AI system capable of doing Jensen's own job. Jensen's agreement signals not just confidence in current capabilities but a willingness to shift the Overton window on what counts as general intelligence, likely to accelerate the AGI narrative across the industry.
  *(Alex Volkov @altryne · 8h · 170K views, 2.2K likes)*

- **Jensen Huang separately urged that every college student should become an AI expert, framing AI literacy not as a specialization but as a universal requirement for graduating into the modern economy.** The statement, clipped by Chief Nerd and gaining 145K views, positions Nvidia as an implicit education platform — its hardware enables the models that every student will need to learn to use.
  *(Chief Nerd @TheChiefNerd · 4h · 145K views, 1.7K likes)*

---

## On-Device AI & Optimization

- **Alexintosh ran Qwen3.5 35B at 13.1 tokens per second on an iPhone 17 (no-pro) — a 2.3x speedup from baseline just two days earlier — using Flash-MoE with fused attention, CMD1+CMD2 merge, fused expert kernel, expert prefetch, and I/O fanout.** This is a Mixture-of-Experts model with 256 experts running fully on-device at conversational speed. The upstream enabler is Apple's increasingly capable Neural Engine combined with aggressive kernel-level optimization. A separate post showed the same model at 5.6 tok/sec on a previous iPhone, making the 13.1 figure a genuine leap.
  *(alexintosh @Alexintosh · 4h · 21K views)*

---

## AI Tools & Products

- **Perplexity Computer can now access real-time options chains and execute live options trades via a free API — enabling users to pull quotes, scan chains, check delta/IV, view portfolios, and place orders all through a single conversation.** This is the first major AI product to integrate real-time financial instrument execution natively, turning a search engine into a brokerage interface. The regulatory and risk implications are significant: conversational options trading eliminates the friction that previously served as a natural guardrail.
  *(Jason Luongo @JasonL_Capital · 6h · 31K views, 316 likes)*

- **OpenArt shipped a browser-based 3D world builder that generates navigable 3D environments from a single prompt or image.** One prompt, and you're walking through a rendered world in seconds. The XR and spatial computing implications are immediate — this collapses the 3D content creation pipeline from days of modeling to seconds of generation.
  *(AI Frontliner @AIFrontliner · 18h · 76K views, 456 likes)*

- **CapCut launched Dreamina Seedance 2.0 — a generate-and-edit video tool rolling out across Southeast Asia, Brazil, and Mexico with plans for broader expansion.** The regional rollout strategy is notable: rather than US-first, ByteDance is seeding its most powerful creative tools in markets where TikTok's creator ecosystem is growing fastest.
  *(CapCut @capcutapp · 4h · 18K views)*

- **MirrorMirror AI launched a marketplace where fashion models license their likeness for AI-generated imagery, creating a new revenue stream that turns model identity into a reusable digital asset.** The approach sidesteps the consent crisis in AI image generation by building licensing into the foundation rather than bolting it on after the fact.
  *(Yusan Lin @yusan_lin · 9h)*

---

## Geopolitics & Markets

- **Iran issued a sweeping ultimatum to Washington — demanding closure of all US bases in the region, a $2M toll for Western ships in the Strait of Hormuz, and $100 billion in reparations — drawing 1.1 million views and 35K likes.** Trump subsequently postponed planned strikes on Iranian power plants after what were described as "very good" talks, extending the Strait of Hormuz deadline. The sequence suggests a high-wire diplomatic dance where maximalist demands create negotiating room.
  *(Furkan Gözükara @FurkanGozukara · 8h · 1.1M views, 35K likes)*

- **Tuki compiled a single-Monday summary that reads like a fever dream: Zuckerberg announced he's building AI to do his own CEO job after firing 31,000 people, while someone purchased $1.5 billion in S&P futures five minutes before Trump halted the Iran strikes.** The juxtaposition captures the surreal velocity of concurrent crises — each item would dominate a normal news cycle, but today they're competing for the same Monday.
  *(Tuki @TukiFromKL · 4h · 450K views, 2.9K likes)*

---

## Wisdom & Observations

- **Garry Tan declared that in the AI revolution, "low status and useful is where the alpha is" — specifically championing markdown files as the ultimate human-AI interface.** His argument: markdown has zero glamour but is readable by humans and models alike, writable, diffable, transformable, and chainable. The observation lands because it names something that power users of Claude Code and similar tools already know intuitively — the most valuable formats in an AI-mediated workflow are the ones nobody would put in a pitch deck.
  *(Garry Tan @garrytan · 11h · 30K views, 586 likes)*

- **Vitrupo cited Stephen Wolfram's observation that AI agents are least useful where expertise is highest, arguing that for experts, thought-to-code is already faster than thought-to-English.** The implication: AI's greatest impact may be in the adjacent competency zones — not replacing experts in their core domain, but making them dangerous in domains they'd otherwise never enter.
  *(vitrupo @vitrupo · 22h · 20K views)*

- **Shankar Padmanabhan presented DiSC, a method for updating LLMs with new world knowledge without undoing skills learned during post-training.** The paper addresses a real pain point: continued training on new facts (2026 knowledge for a 2025-trained model) typically degrades instruction-following and math abilities. DiSC uses document splitting to inject knowledge while preserving capabilities — a quiet but important infrastructure advance.
  *(Shankar Padmanabhan @shankarpad8 · 11h)*

---

*One meta-observation: today's feed is dominated by a single narrative — AI leaving the browser and arriving on the desktop. Claude's computer use announcement, Cowork trending, Jensen's AGI declaration, Qwen on iPhone, Sahil encoding a whole book into executable skills. The common thread isn't any one product launch. It's the moment where AI stops being something you visit and becomes something that lives with you.*

*Compiled by @bag_of_ideas via automated X/Twitter digest*
