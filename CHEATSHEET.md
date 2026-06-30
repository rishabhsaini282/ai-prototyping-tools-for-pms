# AI Prototyping Cheatsheet for PMs

One page. Pin it, print it, or paste it into your team wiki.

## Tool decision matrix

| If you need... | Use | Why |
|---|---|---|
| A fast, polished UI mockup to show design or stakeholders | **v0 (Vercel)** | Generates pixel-perfect, responsive React components straight from a prompt. Fastest path to "here's what the screen looks like." |
| Real interactivity — state, forms, data views | **Lovable** | Handles full-stack logic, not just front-end. Use when the prototype needs to actually *do* something, not just look like something. |
| Something a reviewer can click around in immediately, no setup | **Bolt** | Browser-based execution — generate, run, and test the app without leaving the browser. |

Rule of thumb: start with the *thinnest* tool that proves your point. A v0 mockup that gets stakeholder buy-in beats a Lovable build that took three times as long to prove the same thing.

## Prototype vs. spec — the decision tree

```
Do you need to validate a complex UI interaction, user flow, or core logic?
│
├── YES → Prototype it.
│         Generate the demo, put it in front of real users,
│         use it as the shared reference point with engineering.
│
└── NO → Are you formalizing backend architecture,
          compliance requirements, or final acceptance criteria?
          │
          ├── YES → Write the spec.
          │
          └── NO → You probably don't need either yet —
                    go gather more information first.
```

Prototypes and specs aren't competing artifacts. The prototype proves the idea works before you spend time formalizing it. The spec formalizes what's already been validated.

## What AI prototypes are *not*

- **Not production-ready as-is.** The generated code proves viability; engineering will refactor, secure, and optimize it before it ships. Treat the output as a high-fidelity discovery tool, not a final build.
- **Not a replacement for engineering review.** The handoff conversation changes shape (you're reviewing real code together instead of debating PRD interpretation) but it doesn't disappear.

## 5-question FAQ

**What are AI prototyping tools?**
Platforms that use LLMs to generate functional software demos and UIs from plain-English prompts — interactive, deployable code instead of static wireframes.

**Can a non-technical PM actually do this?**
Yes. The core premise of "vibe coding" is that you don't need a software engineering background or syntax knowledge to generate a working React prototype.

**Bolt vs Lovable vs v0 — which is best?**
There's no single winner. v0 wins on UI speed, Lovable wins on application logic depth, Bolt wins on in-browser execution and testing. Pick based on how technical the demo needs to be.

**Are these prototypes safe to ship as-is?**
No. They're functional and visually accurate enough to prove viability, but engineering teams still need to refactor, secure, and optimize the code before production deployment.

**When should I prototype instead of writing a spec?**
When you're validating complex UI interactions, user flows, or core logic early in discovery. Save the spec for after that validation, when you're formalizing architecture and acceptance criteria.

---
Source: [Stop Writing Specs: Prototype With AI Instead](https://productleadersdayindia.org/blogs/ai-tools-for-product-managers/ai-prototyping-tools-for-pms.html)
