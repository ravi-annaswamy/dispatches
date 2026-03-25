# LinkedIn / Twitter Post — Wednesday Noon Edition, March 25, 2026

---

This morning gave us three things to hold at once.

**1. ARC-AGI-3 launched — and every frontier AI model scored below 1%.**

@arcprize, @GregKamradt, @mikeknoop, and @fchollet put out a benchmark where humans score 100% and the best AI (Gemini 3.1 Pro) scored 0.37%. GPT-5.4: 0.26%. Claude Opus 4.6: 0.25%. Grok: 0.00%.

This isn't a trick benchmark. It's 135 handcrafted environments, fully solvable by ordinary people, designed to test how quickly an AI *learns* something new — not how well it was trained on familiar things. @fchollet calls it the only unsaturated agentic benchmark in the world. @GregKamradt pointed out that models need less and less "prompt harnessing" with each generation — which means the true capability floor is becoming visible for the first time.

**2. Sakana AI's "AI Scientist" was published in Nature.**

@hardmaru and @SakanaAILabs built a system that autonomously runs the full research lifecycle: hypothesize, experiment, write, submit. It's now in the world's most prestigious scientific journal. Peer review accepted a paper where an AI was the primary agent.

These two facts together — AI below 1% on a human learning test AND AI publishing in Nature — describe the same reality from opposite angles. AI is simultaneously more capable and less capable than headlines suggest, depending on exactly what you measure.

**3. Google TurboQuant cut LLM memory 6x. Chip stocks fell 7-8%.**

@GoogleResearch published a compression algorithm that reduces LLM key-value cache memory by at least 6x with zero accuracy loss. Micron dropped 6.82%, Sandisk fell 8.30%. @rasbt and @altryne immediately pushed back: this won't reduce memory demand, it will enable bigger models (Jevons' Paradox for AI hardware). Both are probably right — just on different time horizons.

---

The pattern I keep seeing: every efficiency breakthrough gets absorbed by the next layer of ambition. Every capability gap that seems decisive gets quietly solved somewhere else while everyone is watching the gap.

The only honest position is to watch both at once.

**If you're running LiteLLM in production: @ishaan_jaff confirmed a supply chain attack on PyPI versions 1.82.7 and 1.82.8 — packages have been pulled, pin to a safe version now.**

Full digest: ravi-annaswamy.github.io/dispatches

#AI #MachineLearning #ArtificialIntelligence #ARCAGI #LLM #AIResearch
