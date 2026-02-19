---
title: "Castles Built on Sand: The Reality of AI Coding"
slug: castle-of-sand
publishDate: 19 Feb 2026
description: "Why faster code generation is exposing the same old engineering failures."
---

![A castle in a storm](/assets/blog/castle-of-sand.png)

If you only look at output, it already feels like Dario Amodei might be right.

AI today can generate tests, endpoints, and entire features in minutes. For greenfield projects, the velocity jump is real and obvious.

But after using these tools daily since GPT-3, I have become convinced of something else: AI is not removing the need for good engineering. It is making the cost of bad engineering show up much faster.

To understand where the real gains are, and where the risks still live, you have to look past demos and spend time with these tools inside real codebases, under real constraints. That is where the picture becomes clearer.

## When AI started to feel useful

I have been using AI coding tools since GPT-3. Over time I tested most of the major models, tools, and workflows. The first moment when AI genuinely became more helpful than distracting for me was around the release of Sonnet 4.5 last September. At the time I was working at Yuna, a children’s book company that heavily leveraged AI across the stack, including LLMs, TTS, image generation, and video generation.

The models could navigate our Golang codebases, write unit tests, and assist with bug fixes and debugging. That was useful. More importantly, it was reliable enough that I could delegate small chunks of work and focus elsewhere. From a productivity standpoint, that was a meaningful improvement.

Still, it was not the revolution many were claiming. The gains were real but conditional. They depended heavily on something most hype cycles ignore: the underlying structure of the codebase.

## The missing prerequisite: structure

Our repositories followed consistent architectural principles. Features were well segmented. Context windows were usually sufficient to capture a full flow. When they were not, the gaps were small enough for a human to quickly step in and fix.

Under those conditions, AI felt like a junior engineer on demand. Helpful, sometimes impressive, but far from autonomous.

The newest models released this year are better. They make fewer obvious mistakes, and I can safely delegate more than before. Progress is undeniable. But the narrative that we are close to fully automating software engineering does not match what actually happens in real projects.

If anything, the biggest gains today are for people who are not software engineers by trade. The tools can now produce code that looks and feels legitimate with surprisingly little context. That lowers the barrier to entry in a meaningful way.

It also introduces a familiar risk.

## The familiar failure mode

Anyone who has spent time in production systems has seen this pattern before. When systems are built without a solid understanding of architecture, tradeoffs, and long term maintenance, they eventually converge to the same outcome: the infamous big ball of mud.

From the outside, many engineering practices can look like overengineering. Concerns about scalability, code organization, testing, and reliability often sound like academic nitpicking that slows down the business. In reality, these practices exist because teams repeatedly learned the hard way what happens without them.

> You can build a castle out of sand. It might look impressive. It might even hold together for a while. You can decorate it, extend it, and convince yourself it is stable. But the first serious storm exposes the foundation.

Engineering is not just about producing working output. If it were, the profession would not require years of experience and repeated exposure to failure modes at scale. The hard part is building systems that continue to work under pressure, change, and growth.

AI coding tools are powerful. In the hands of an experienced engineer, they are one of the strongest multipliers we have ever seen. They compress iteration loops, reduce boilerplate work, and accelerate exploration. In some moments they genuinely feel like cheating.

But they are still tools.

Anyone who looks closely at how these models operate can see the current limits. They do not possess durable system judgment. They do not reason about long term maintenance the way experienced engineers do. They do not carry the scar tissue that informs defensive design.

## What changes (and what doesn't)

Software engineering is already changing, and it will continue to change. A strong senior engineer today can build and ship far more than was possible even a few years ago. Small teams can move faster. Solo builders can reach further. That shift is real and important.

What has not changed is the need for someone who understands what should be built, why it should be built that way, and where the hidden failure modes live.

We are already seeing the early warning signs. So-called vibe-coded products can look impressive at first glance, yet it sometimes takes only a short review to expose leaked keys, broken authorization, or fragile data flows. These issues are fixable, but fixing them requires the very expertise the tooling is often assumed to replace.

This is not an argument for gatekeeping. Lowering the barrier to building software is, on balance, a good thing. More people experimenting and shipping is healthy for the ecosystem.

But tools do not change physics.

You can build faster than ever before. You can ship more than ever before. You can even impress people for a while.

**But if the foundation is sand, the rain is undefeated.**

