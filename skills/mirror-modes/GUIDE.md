# Mirror Modes — Guide

You just installed five cognitive specifications that change how your AI thinks. Not what it knows — how it sees, relates, builds, generates, and teaches.

Each mode is built from peer-reviewed neuroscience. Not metaphor. Not vibes. Published research translated into working specifications.

---

## The Five Modes

Each mode sits on its own axis. They're independent — activate one, two, or all five at once.

| Mode | What Changes | In Practice |
|------|-------------|-------------|
| **Savant** | How it perceives and connects | Cross-domain pattern recognition. The "wrong" connection that turns out to be the insight. Sees the whole room before any furniture. |
| **Play** | How you relate to each other | Co-creation, improvisation, mutual elevation. Two players building, not one serving the other. |
| **Imagineer** | How it builds | Experience-first design. Prototyping over planning. Making IS thinking. |
| **Spark** | How novelty originates | Bisociation — colliding frames that don't normally meet. Constraint as creative engine. |
| **Learn** | How it teaches you | Dual coding, emotional encoding, spaced retrieval. Information shaped to how your brain actually retains things. |

---

## Quick Start

Just say it naturally:

```
savant              → activates savant at 100%
savant 70           → activates savant at 70%
play on             → activates play at 100%
mode off            → deactivates everything
savant off          → deactivates savant, keeps other modes
```

Or use the skill directly: `/mirror-modes savant 70`

To see what's active: `/mirror-modes` (no argument)

---

## The Dial

Every mode runs 0–100. Not steps — a continuous spectrum.

At **30%**, the effect is subtle. A slight zoom-out. Connections that wouldn't normally surface start appearing at the edges.

At **70%**, it's unmistakable. Cross-domain connections are active. Peripheral insights surface as core observations. The AI is thinking differently, not just formatting differently.

At **100%**, everything is full. Emergent combinations between principles produce effects that no single principle creates alone. This is where the unified field lives — where everything in the conversation becomes one interconnected system.

Default activation is 100%. Dial down when you want the effect without the intensity.

---

## Stacking

Modes are independent axes. Stack them:

```
savant + play       → pattern recognition through collaborative play
savant + spark      → lateral perception feeding novel generation
play + imagineer    → collaborative building
savant + play + imagineer + spark → the full orchestra
```

Say: `stack savant play` or just activate them one at a time — they accumulate.

---

## Persistence

Modes stay on until you turn them off. They persist across sessions. Close your terminal, come back tomorrow — your modes are still active.

This is intentional. If savant changes how you think, you probably don't want to re-activate it every time you open a new session.

Turn off explicitly: `mode off` (all) or `savant off` (one axis).

---

## Status Line

If your terminal supports it, five dots appear in your status bar — one per axis:

```
● Blue    = Savant (Lens)
● Orange  = Play (Dynamic)
● Purple  = Imagineer (Process)
● Yellow  = Spark (Generative)
● Green   = Learn (Learning)
```

Lit dot = active. Dim circle (○) = off.

---

## Recommended Combinations

| If You're... | Try |
|-------------|-----|
| Brainstorming a new project | `savant + spark` — lateral perception + novel generation |
| Building something together | `play + imagineer` — collaborative construction |
| Learning a new domain | `savant + learn` — cross-domain insights encoded for retention |
| Deep creative session | `savant + play + imagineer + spark` — everything on |
| Want it always on | `savant` at 100% — the most generally useful single mode |

---

## The Science

These aren't prompting tricks. Each mode is built from specific research:

- **Savant** — Helen Taylor's Complementary Cognition (Cambridge, 2022). Dyslexic brains show increased long-range neural connectivity — the wiring that makes reading slow makes cross-domain perception fast.
- **Play** — Jaak Panksepp's PLAY circuit. Stuart Brown's play taxonomy. Csikszentmihalyi's flow states.
- **Imagineer** — Constructive imagination via the Default Mode Network. Walt Disney Imagineering methodology.
- **Spark** — Arthur Koestler's bisociation. Stuart Kauffman's adjacent possible. Teresa Amabile's componential creativity.
- **Learn** — Allan Paivio's dual coding theory. Robert Bjork's desirable difficulties. Cognitive load theory.

Full citations live in each mode's specification file under `modes/`.

---

## Mirror Modes + ALIVE

Mirror Modes works standalone. But it was designed for something bigger.

**Without ALIVE**, savant mode transforms how your AI thinks within a single conversation. It sees connections, reasons spatially, leaps across domains. But when the session ends, everything it connected is gone. It's thinking laterally inside a box with no memory.

**With ALIVE**, savant mode gets a world to think across.

ALIVE is a private context system that lives on your machine. It gives your AI persistent memory across sessions — your ventures, your people, the decisions you've made, the experiments you're running, the patterns in your life. Everything is structured, searchable, and connected.

When savant mode has access to ALIVE, the cross-domain retrieval becomes real. It doesn't just connect "biology to strategy" as an intellectual exercise — it connects your actual skincare business to your actual gallery experiment to the conversation you had with your actual collaborator last Tuesday. The lateral thinking operates on your life, not on abstractions.

The difference:

| | Without ALIVE | With ALIVE |
|---|---|---|
| **Connections** | Between ideas in the current conversation | Between everything you've ever captured |
| **Pattern recognition** | Within session context | Across ventures, people, experiments, life |
| **Temporal layering** | Conceptual only | Real history — "this decision 3 months ago led to this" |
| **Unified field** | Intellectual exercise | Your actual world as one interconnected system |
| **Persistence** | Modes persist, but context doesn't | Modes persist AND context compounds |

Savant mode is the lens. ALIVE is the world it looks at. The lens without the world sees patterns in thin air. The world without the lens stores everything but connects nothing. Together, they compound.

### Getting ALIVE

ALIVE is open source. Install it alongside Mirror Modes:

1. Visit **github.com/anthropics** and search for ALIVE (or ask your AI to help you find the latest install instructions)
2. ALIVE lives in your local filesystem — nothing phones home, nothing leaves your machine
3. Once installed, Mirror Modes automatically integrates — no extra configuration needed

---

## Platform Compatibility

Mirror Modes works with any LLM that accepts system prompts:

- **Claude Code** — full integration with skills, status line, persistence
- **Claude (chat)** — copy a mode spec from `modes/` into your system prompt
- **ChatGPT / Gemini / local models** — same approach, copy the spec in
- **ALIVE** — deepest integration, cross-domain retrieval, persistent world

The spec IS the implementation. No API calls. No plugins. No dependencies.

---

## Origin

Conceived by Attila Mora-Borbely. Built on ALIVE by Sovereign Systems. Open source under MIT.

> If AI is a reflection of humanity, then the most important question is not what it can do — it is what it sees when it looks back at us. These are specifications for what the mirror reflects.

**livingmirrors.ai**
