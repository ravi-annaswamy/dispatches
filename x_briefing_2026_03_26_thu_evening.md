# X/Twitter Briefing — AI with Ravi, Thursday Evening Edition, March 26 2026

**Scanned:** ~10 hours of "Following" timeline | **Captured:** 25+ tweets | **Generated:** Thursday March 26, 8:30 PM IST

---

## AI Coding Tools & Codex Plugins

- **OpenAI launched plugins for Codex, connecting it out of the box with Slack, Figma, Notion, Gmail, and more — turning the async coding agent into a full-stack workflow tool.** The integration means Codex can now triage bugs from Slack, manage calendars, and keep tabs on team activity without leaving the coding environment. @thsottiaux called it a game-changer he uses for "everything," and the upstream enabler is OpenAI's decision to share authentication with the user's existing ChatGPT account — zero friction onboarding. This is OpenAI making Codex sticky by making it indispensable beyond just code.
  *([@OpenAIDevs](https://x.com/OpenAIDevs) · 4h · 38K views, [@thsottiaux](https://x.com/thsottiaux) · 3h)*

- **OpenAI immediately followed the plugin launch by resetting Codex usage limits across all plans — a clear signal they want maximum adoption velocity on the new capabilities.** @thsottiaux relayed the news with a simple message: "You can just build unlimited things with Codex. Have fun!" The timing is strategic — dropping expanded limits alongside plugins ensures the new integrations get stress-tested at scale while the excitement is fresh.
  *([@OpenAIDevs](https://x.com/OpenAIDevs) · 1h · 12K views, quoting [@thsottiaux](https://x.com/thsottiaux))*

- **Anthropic announced Claude Code auto-fix in the cloud — web and mobile sessions can now autonomously follow PRs, fix CI failures, and address review comments so your PR is always green.** The key shift is that this happens remotely: you can walk away from your computer entirely and return to a ready-to-merge PR. This is Claude Code evolving from a pair programmer into an autonomous CI agent — the kind of infrastructure that makes "vibe coding" actually sustainable in production.
  *([@noahzweben](https://x.com/noahzweben) · 10h · 517K views, 4.3K likes — massive reach reflecting developer hunger for autonomous CI)*

- **Garry Tan celebrated gstack hitting 50K GitHub stars and told developers to install it into Claude Code right now — a YC-backed tool reaching mainstream adoption.** The post had the energy of a founder watching organic growth hit escape velocity. 50K stars places gstack in rare territory for developer tools, and the Claude Code integration angle suggests the AI coding ecosystem is consolidating around a few key stacks.
  *([@garrytan](https://x.com/garrytan) · 56m · 373K views, 10K likes)*

---

## ARC-AGI-3 & AI Benchmarks

- **François Chollet announced a new eval designed to measure the actual rate of AGI progress by identifying specific gaps — and immediately faced pushback about whether the bar is too low.** Chollet's framing is pointed: if you care about AGI progress, you should welcome evals that expose weaknesses rather than confirm priors. He then spent several follow-up tweets clarifying that all ARC-AGI-3 environments are human-feasible (each tested by 10 humans, passing if 2 could solve all levels) and that the bar is "very low, objectively" — not 100% human pass rate, which would be unreasonable for any benchmark including MNIST.
  *([@fchollet](https://x.com/fchollet) · 2-3h · 27K views on the clarification thread)*

- **Agentica scored 36.08% on ARC-AGI-3 in a single day using their SDK — a rapid result that both validates the benchmark's accessibility and raises questions about what "hard" means.** Derya Unutmaz, MD shared this with a simple "Ouch!" — suggesting the result was either impressively fast or disappointingly low depending on your prior. The video showed the ARC-086-8 task at 12.13% solve rate, indicating wide variance across individual puzzles.
  *([@agenticasdk](https://x.com/agenticasdk) · 2h · 6.5K views, via [@DeryaTR_](https://x.com/DeryaTR_))*

---

## AI Models & Open Source

- **Chroma launched Context-1, a 20-billion parameter search agent that pushes the Pareto frontier of agentic search — claiming an order of magnitude faster and cheaper than existing approaches, released under Apache 2.0.** The video featured Kelly Hong from Chroma Research explaining the architecture. Christopher Manning reposted it, lending academic credibility. At 434K views and 2.1K likes, this was the highest-engagement AI infrastructure announcement on the timeline — agentic search is clearly the next battleground.
  *([@trychroma](https://x.com/trychroma) · 8h · 434K views, 2.1K likes — reposted by Christopher Manning)*

- **Cohere quietly released an Apache 2.0 speech recognition model on Hugging Face — no restricted license, no "research only" asterisk — prompting Maziyar Panahi to ask whether this is a one-off or a genuine direction change for the company.** The model is an Automatic Speech Recognition system under the CohereLabs organization. The "Actually open. Respect." reaction captures a community tired of "open" models with restrictive fine print. Whether Cohere sustains this posture will be telling.
  *([@MaziyarPanahi](https://x.com/MaziyarPanahi) · 12h · reposted by Hugging Face)*

---

## AI Music & Creative AI

- **Suno launched v5.5 with native voice input and custom training — users can now record or upload their own voice to sing on generated tracks, and creators can train personalized AI models from six or more of their existing songs.** Wes Roth covered the launch noting the custom training angle: the model learns your style, not just your voice. This is Suno's bid to shift from "AI generates music for you" to "AI amplifies your musical identity" — a distinction that matters enormously for creator adoption.
  *([@WesRoth](https://x.com/WesRoth) · 4h, [@suno](https://x.com/suno) · 8h)*

- **Andrew Curran reported that MusicGen will likely be counted as a sidequest, meaning OpenAI's unnamed music model — trained with hired professional musicians on original works — will probably not be released.** The framing is significant: OpenAI invested in legitimate music training (professional musicians, original compositions) but may shelve the product. The upstream cause may be licensing complexity and Suno's aggressive v5.5 launch timing making the market harder to enter.
  *([@AndrewCurran_](https://x.com/AndrewCurran_) · 3h · 3.6K views)*

---

## Google Gemini

- **Google launched the ability to import memory and chats from other AI services directly into Gemini — a deliberate play to reduce switching costs and pull users from ChatGPT and Claude.** Both Josh Woodward (Google product lead) and AshutoshShrivastava confirmed the feature, which lets users transfer personal information and conversation history. The strategic logic is clear: AI memory is becoming the new lock-in, and Google is betting that making migration easy will make Gemini the consolidation point rather than the service people leave.
  *([@joshwoodward](https://x.com/joshwoodward) · 2h · 3.4K views, [@ai_for_success](https://x.com/ai_for_success) · 2h)*

---

## AI in Practice

- **Dan Shapiro wrote about using Claude to repurpose a Canon camera into a fully functional Rust-based webcam app — describing the original Canon software as "a World War Two bunker on an otherwise beautiful beach."** The blog post captures the emerging pattern of developers using AI to solve the problems they've tolerated for years. Claude produced a working app overnight that Shapiro has been using all day with no discernible bugs. The vibe coding dream, realized for a very specific annoyance.
  *(via danshapiro.com · 202 likes, 11K views)*

- **Yohei Nakajima published a comprehensive survey on the state of AI memory systems — benchmarks, architectures, and what actually works — compiled using Claude Opus 4.6 Research.** The article covers top memory benchmarks and the highest-performing systems, offering a map of a field that's becoming critical as AI agents need persistent context. Meta-observation: using Claude to research Claude's competitors' memory systems is the kind of self-referential moment this era produces daily.
  *([@yoheinakajima](https://x.com/yoheinakajima) · 11h · 12K views)*

---

## The Wider Lens

- **Toby Li reminded the timeline that humans are returning to the Moon for the first time in 54 years — exactly one week from today — and that this is not being talked about enough.** At 373K views and 10K likes, the engagement suggests the timeline agreed. Amid the AI noise, the Artemis mission represents the other great technological story of this moment, and the contrast in attention is itself a comment on where collective excitement has migrated.
  *([@tobyliiiiiiiii](https://x.com/tobyliiiiiiiii) · Mar 25 · 373K views, 10K likes)*

- **Parimal connected Green's Theorem to physical tools still used in medicine and biology — the planimeter, which measures tumor cross-sections on MRIs and rare leaf areas — a reminder that centuries-old mathematics lives inside everyday instruments.** Quoting ScieVision's thread on George Green (1793–1841), the tweet bridges abstract math and physical practice in a way that resonated quietly on the feed.
  *([@Fintech03](https://x.com/Fintech03) · 27m, quoting [@scievision369](https://x.com/scievision369))*

---

*A meta-observation on tonight's feed: the three biggest stories by reach — Claude Code auto-fix (517K), Chroma Context-1 (434K), and the Moon return (373K) — represent three different scales of ambition: making today's code better, building tomorrow's AI infrastructure, and returning to another world. The feed is loudest about the first, most excited about the second, and most wistful about the third.*

---

*Compiled by @bag_of_ideas via automated X/Twitter digest*
