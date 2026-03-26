# X/Twitter Briefing — Thursday Noon Edition, March 26 2026

**Scanned:** ~8 hours of "Following" timeline | **Captured:** 25+ tweets | **Generated:** Thursday March 26, 12:00 PM

---

## Gemini 3.1 Flash Live Drops

- **Google launches Gemini 3.1 Flash Live — its biggest upgrade to real-time voice AI — with 2x longer context, noise filtering, and dynamic tone matching.** Josh Woodward announced the model powers Gemini Live on both Android and iOS, calling it faster, smarter, and more emotionally intelligent. The upstream enabler is Flash's efficiency profile: Google is betting that a mid-tier model with excellent latency beats a frontier model that stutters. This positions Gemini Live as a genuine daily-driver voice assistant, not just a demo.
  *(via @joshwoodward · 19m, 179 likes — reposted by @GeminiApp)*

- **Logan Kilpatrick says the team spent over a year improving the model, infrastructure, and experience — and the result is a "step function" in real-time AI.** The emphasis on infrastructure investment signals that Google sees voice+vision agents as a core product surface, not an experiment. The Big Bench Audio charts shared by early-access tester Ashutosh Shrivastava show Flash Live leading all competitors on speech recognition accuracy at 97%.
  *(via @OfficialLoganK · 56m, 45 likes; @ai_for_success · 49m)*

---

## The Vibe Coding Reckoning

- **Andrej Karpathy says the hardest part of building his app MenuGen wasn't the code — it was the DevOps: payments, auth, database, security, domain names, "like IKEA furniture you have to assemble."** Patrick Collison quote-tweeted Karpathy's original blog post about vibe coding being exhilarating locally but a slog to deploy. The implication is sharp: AI can now write application logic fluently, but the unglamorous plumbing of real deployment remains stubbornly human. This is the new bottleneck.
  *(via @karpathy · 4m, quote-tweeting @patrickc · 43m, 104 likes, 6.9K views)*

- **Carlos E. Perez argues Karpathy's recent No Priors interview is more radical than most summaries suggest — he's not saying AI is a better tool, he's saying the structure of knowledge work itself is changing.** The key quote: "Code's not even the right verb anymore." When someone at Karpathy's level reframes the vocabulary, pay attention — it usually means the old mental model has already broken.
  *(via @IntuitMachine · 1h, 11 likes, 1.2K views)*

- **Ethan Mollick revisits a year-old prediction that AI would write 100% of code within 12 months — and notes it's either hype or a startlingly solid call, since Claude Code now writes a remarkable percentage.** His sharper point: "Adoption is more of a barrier than technology." The tools are ready; the organizations are not. This Jevons-paradox framing connects directly to Chollet's observation below.
  *(via @emollick · 3h, 241 likes, 24K views)*

- **François Chollet responds to Aaron Levie's Jevons paradox claim with a crisp prediction: "There's going to be a lot more software, and a lot more demand for software engineers. And a lot more token consumption."** Levie's original point — that non-tech companies are now tackling software projects they never could before — is the demand-side story. Chollet adds the supply-side corollary: when software gets cheaper to write, the world wants infinitely more of it.
  *(via @fchollet · 2h, quoting @levie, 208 likes, 17K views)*

- **An immunologist with no formal CS training says he launched a complex science app with OpenAI's Codex overnight and "just froze, staring at the screen" in disbelief.** Derya Unutmaz, MD was quote-tweeting JB's Uncivilized.fun — a Civilization clone with natural-language AI diplomacy built in 48 hours of vibe coding. The pattern: domain experts are shipping real software with conversational AI, and the gap between "toy demo" and "actual product" is collapsing.
  *(via @DeryaTR_ · 3h, quoting @jamie247, 70 likes, 7K views)*

A meta-observation: five separate voices in the last 8 hours — Karpathy, Chollet, Mollick, Perez, and Unutmaz — all independently converged on the same conclusion from different angles. The coding paradigm shift isn't a prediction anymore. It's a Wednesday.

---

## ARC-AGI-3 and the Benchmark Wars

- **Greg Kamradt reports that 12 hours into the ARC Prize 2026 Kaggle competition, the human-set high score is still below the template baseline — with Stochastic Goose leading at 0.25.** François Chollet's ARC-AGI-3 benchmark launched yesterday to crush current AI models, and early signs suggest it's working. The leaderboard's low scores indicate the benchmark is genuinely measuring something frontier models can't yet brute-force.
  *(via @GregKamradt · 9h, reposted by Ravi)*

- **Jia-Bin Huang highlights the power of medium: a research paper on arXiv had 2 citations after 11 months, but an accessible blog post about the same work hit 12 million views in one day.** The quoted work is Google Research's TurboQuant — a compression algorithm that reduces LLM key-value cache memory by 6x with zero accuracy loss. The science was always there; the blog post just let people find it.
  *(via @jbhuang0604 · 14h, reposted by Christian Langreiter)*

---

## AI Infrastructure & Capital Flows

- **A Morgan Stanley diagram mapping OpenAI's ecosystem capital flows went viral — showing how revenue and investment cascade through Microsoft, Oracle, Coreweave, Amazon, Nvidia, and AMD.** Lydia DePillis called it "hell of a graphic," and 257K people agreed. The diagram makes visible what's usually abstract: OpenAI sits at the center of a financial web where compute dollars flow down through cloud providers to chip makers to data center lessors. It's the AI economy in one picture.
  *(via @lydiadepillis · 20h, reposted by @fastml_extra, 4.1K likes, 257K views)*

- **Cloudflare discovered that a one-line Kubernetes config change — adjusting fsGroupChangePolicy — reduced their Atlantis instance restart time from 30 minutes to 30 seconds, saving 600 hours a year.** The fix is absurdly simple (one config field), which is exactly the point: infrastructure complexity is now so deep that million-dollar savings hide in single-line changes nobody thinks to look for.
  *(via @Cloudflare · 3h, 64 likes, 16K views)*

---

## Local AI & Privacy-First Tools

- **Niels Rogge demonstrates running Nvidia's NemoClaw with Qwen3.5-27B entirely locally via Telegram — no API costs, no data leaving the device.** NemoClaw is a security sandbox built on top of OpenClaw that restricts file and network access for the AI agent. The video shows a complete agentic assistant running on consumer hardware through a chat interface people already use. The upstream enabler: open-weight models are now good enough that the "local vs. cloud" tradeoff has genuinely tipped for many use cases.
  *(via @NielsRogge · 2h, reposted by AK, 185 likes, 20K views)*

---

## Brain-Computer Interface Milestone

- **Neuralink's ALS patient Kenneth Shock progressed from attempting to speak aloud, to silently thinking words, to having his brain implant decode them into speech — using ML to map neural activity to phonemes.** Wes Roth detailed how Kenneth received the N1 implant in January 2026 and is now part of Neuralink's VOICE clinical trial. The key technical advance is phoneme-level neural decoding, which means the system learns the smallest units of sound rather than whole words — making it far more generalizable.
  *(via @WesRoth · 3h, quoting @neuralink, 17 likes, 1.7K views)*

---

## The Lighter Side & Quotables

- **An AI detector (ZeroGPT) flags Abraham Lincoln's Gettysburg Address as 96.2% AI-generated — a perfect illustration of why these tools remain unreliable.** Rohan Paul shared the screenshot that proves well-crafted human prose triggers the same statistical patterns these detectors look for. The tools are measuring "sounds like GPT" rather than "was made by GPT."
  *(via @rohanpaul_ai · Mar 25, reposted, 74 likes, 26K views)*

- **Richard Dawkins turns 85 on #ScienceAppreciationDay and reminds his followers that without science, they probably wouldn't have reached their latest birthday.** A characteristically crisp framing on a day that shares his birthday.
  *(via @RichardDawkins · 33m, 184 likes, 7.4K views)*

- **Alec Stapp's reminder that the US lost the 5G race because it didn't give one Turkish mathematician a green card hit 100K views.** Erdal Arikan solved a fundamental problem in information theory at Caltech/MIT, couldn't find a US employer, returned to Turkey — and Huawei used his discovery to build one-third of the world's 5G infrastructure. 100K views suggests the immigration-innovation connection still resonates viscerally.
  *(via @AlecStapp · 3h, reposted by @garrytan, 2.9K likes, 100K views)*

---

*Compiled by @bag_of_ideas via automated X/Twitter digest*
