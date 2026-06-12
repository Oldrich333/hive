# Hive

**An autonomous business operations platform. AI agents run the business; the human owns the vision.**

> Status: **preview**. This repo is an announcement, not a release. No code here yet — the platform is running in production, privately, and we're deciding what gets opened and how. If you're building something similar, we want to hear from you — see [Get in touch](#get-in-touch).

## What this is

I'm not a programmer. Yet today, AI agents run my companies' day-to-day operations — marketing, infrastructure, customer channels, research, content — end to end. I set direction; the system executes, verifies its own work, fixes what breaks, and asks me only the questions that are genuinely mine to answer.

Hive is the platform that makes that possible. It's been built almost entirely *by* the agents that run on it, which we consider its core property, not a curiosity: a platform whose agents extend it — writing their own connectors, tools, and guardrails as the business needs them.

## The bet

> **Output quality is a function of context quality and input structure — not model intelligence.**

Everyone is waiting for smarter models. We found the constraint is elsewhere. Today's models already solve most of what a real business needs — *if* the system around them maintains a precise, current, machine-readable picture of the world and feeds them exactly the context each decision needs. So that's what Hive is: not a chatbot wrapper, but a context engine with agents on top.

What that looks like in practice:

- **A living catalog** — the company's entire operational state as a tree of human- and machine-readable dossiers, continuously updated by the agents themselves. The catalog, not any model's memory, is the source of truth.
- **Goal engine** — give it a goal (research, code, content); it iterates — plan, execute, judge, polish — until the result actually holds, not until it merely sounds done.
- **Self-extension** — when an agent needs a capability that doesn't exist, it builds it, reviews it adversarially, and hardens it against recurrence of whatever failed.
- **Multi-tenant** — one platform, many businesses, each with its own catalog, channels, and governance phase (from "approve everything" to "notify me on critical only").
- **Discipline over genius** — adversarial multi-model review of changes, secret-safe I/O, monitors that turn incidents into permanent guardrails. The platform absorbs its failures into resilience.

## Already public

We extract the generally useful pieces as we go:

| repo | what |
|---|---|
| [smart-read](https://github.com/Oldrich333/smart-read) | token-efficient file read/grep/glob for agents + MCP server |
| [ax-headers](https://github.com/Oldrich333/ax-headers) | one-line machine-readable Python file headers |
| [raisin](https://github.com/Oldrich333/raisin) | Python LLMs read at ~50% of the tokens |
| [hard-compact](https://github.com/Oldrich333/hard-compact) | compact prompts that don't lobotomize your CLI agent |
| [full-review](https://github.com/Oldrich333/full-review) | adversarial code review skill |

More will follow. The intention for the platform itself is **open-core**: the engine open, under a license that keeps it open.

## Where this is going

A worker you own, not an agent you rent. Your data in files you can read, on machines you control, in formats that aren't hostage to us or anyone. The work-saving that AI brings should land with the people doing the work.

That's the direction. The product comes first; the manifesto when it's earned.

## Get in touch

If you're building autonomous business operations, agent platforms, context/memory engines, or self-extending agent systems — or running a real business on agents and hitting the same walls we did:

- open an [issue](../../issues) or [discussion](../../discussions) here,
- or write to **dvorak@oldrich.me**.

We're especially interested in comparing notes on: catalog/state architectures for agents, agent self-extension with safety, multi-model adversarial review, and long-horizon goal loops.

---

*No code yet. Watch the repo.*
