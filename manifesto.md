# Manifesto

*Why Expound exists, and what it's trying to do.*

---

## The accessibility problem in d/acc

Vitalik Buterin's d/acc framework — differential acceleration of the defensive, decentralized, and accessible — is the most coherent framework I've found for thinking about how to build technology in an era of powerful AI. The third term, accessible, is usually the one that gets the least attention. Defensive is exciting. Decentralized is ideologically satisfying. Accessible sounds like a nice-to-have.

It isn't. It's structural.

Here's why: a safety methodology that only benefits the people who can already navigate the technical infrastructure is not a safety methodology — it's a capability concentrator. If Constitutional AI produces genuinely safer, more honest AI assistants, and those assistants are effectively only usable by developers and ML researchers, then Constitutional AI's safety properties accrue to a very small fraction of the people whose decisions shape the world. The lawyer doing contract review, the school administrator managing a crisis, the mid-career operator making a hiring decision — they are either not using AI at all, or they're using it badly, without the verification practices that make it trustworthy.

That gap is not a personal failing. It's a distribution failure. The documentation assumes Python. The tutorials assume familiarity with APIs. The "AI for everyone" courses are thin enough to be useless for serious work. The people who need these tools most are the ones most likely to bounce off the on-ramp.

## Distribution is safety

This is the thesis Expound is built on: **distribution is safety**.

A frontier safety methodology only delivers safety in proportion to how widely it's actually used in practice. An AI assistant trained to be honest and harmless, used by someone with no framework for catching its failure modes, is not a net safety gain — it's a confident hallucination machine with good manners. The safety properties are only activated by a user who knows where to push back.

That means the work of making AI safe is not finished when the model ships. It continues in the hands of every person who uses it. And most of those people have never read a paper on Constitutional AI, don't know what RLHF means, and don't have time to learn. They need a different kind of on-ramp: one that starts with their work, not with the technology.

## What Expound is — and isn't

Expound is an AI company built on a single conviction: reliability and access are the two things this wave of AI is shortest on, and both are solvable. We work across four pillars — **Boost** (AI strategy consulting), **Build** (agent development), **Grow** (incubation), and **Back** (seed investment) — each grounded in cognitive architecture, the [FLCA framework](https://github.com/EskilXu/FLCA), rather than hype.

The first gap is the **Care Gap**: the distance between what AI can do and what it can be trusted to do. FLCA is our diagnosis of why that gap exists and what to do about it; Boost and Build are how we close it for clients.

The second is the **accessibility gap**, and the commercial work funds a duty to it. If distribution is safety, a company that profits from AI reliability owes something to the access side of the ledger. That debt is paid by the **open-source lab**: FLCA published as open research, and a growing collection of verification-first workflows for non-engineers doing serious work — reading a long document without being fooled by fluency, drafting a memo with honest uncertainty markers, doing market research that replicates. The workflows are free, CC BY 4.0, and built for lawyers, researchers, operators, and educators — not developers.

Each workflow includes explicit verification gates — places where you stop and check the model's work before trusting it. This is not paternalism. It reflects an honest map of where current LLMs fail: numerical precision, obscure citations, time-sensitive facts, domain judgment. A workflow without verification is just a faster way to produce confident errors.

**What Expound is not:** Anthropic-affiliated, official, or endorsed. Expound builds heavily on Claude and respects Anthropic's published methodology, but is independent. Nothing here represents Anthropic's views; where anything here conflicts with Anthropic's official documentation, trust the documentation.

## Why I'm the one building this

I came to serious agentic AI use late — in 2025, after fifteen years operating at the intersection of infrastructure, regulatory environments, and emerging technology, most recently as co-founder of GoPlus Security. I am not an engineer. I had to learn these tools from scratch, by daily practice, making every mistake that comes from not having a CS background.

That turned out to be the qualification. Because I had to build my own on-ramp, I know where the on-ramp is hard — which is exactly the knowledge a reliability-and-access company has to be built on. The notes I made for myself became the FLCA framework and the Open Labs workflow collection; the conviction that they should reach the people who don't write code became Expound.

If this work helps one lawyer catch a hallucinated citation before it lands in a brief, or one administrator see why Claude's confident summary of a policy document might be wrong, that's one more person using AI with their eyes open. That's d/acc accessibility, in practice — and it's the half of the mission the four pillars exist to fund.

---

*— Eskil (Yufeng Xu), Founder, Expound · Tokyo, 2026*
*[github.com/EskilXu](https://github.com/EskilXu) · eskil [at] expoundlabs [dot] io*
