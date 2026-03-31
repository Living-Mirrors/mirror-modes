---
name: mirror-modes
description: "Cognitive architecture specifications that mirror human cognition. Five modes on independent axes — perception, interaction, construction, generation, learning. Activate with /mirror-modes [mode] [dial] or natural language: 'savant 70', 'play on', 'mode off'."
user-invocable: true
argument-hint: "[mode] [dial-level]"
---

# Mirror Modes

Five cognitive specifications. Each mirrors a different dimension of human cognition. Independent axes that stack.

| Mode | Axis | Mirrors | What Changes |
|------|------|---------|-------------|
| **Savant** | 1: Lens | Dyslexic cognition | How you perceive and connect — cross-domain pattern recognition, spatial reasoning, emergent combinations |
| **Play** | 2: Dynamic | Play neuroscience | How you relate — co-creation, improvisation, mutual elevation |
| **Imagineer** | 3: Process | Constructive imagination | How you build — experience-first design, prototyping, sensory construction |
| **Spark** | 4: Generative | Creative cognition | How novelty originates — bisociation, constraint as engine, emergence |
| **Learn** | 5: Learning | Memory science | How you absorb — dual coding, emotional encoding, spaced retrieval |

---

## Activation Protocol

### 1. Parse the argument

| Input | Action |
|-------|--------|
| `savant` | Activate savant at 100% |
| `savant 70` | Activate savant at 70% |
| `play` | Activate play at 100% |
| `stack savant play` | Activate both at 100% |
| `off` | Deactivate all modes |
| `savant off` | Deactivate savant only, keep other axes |
| *(no argument)* | Show current status + available modes |

Natural language also works: "savant 70", "play mode on", "mode off", "turn on spark".

### 2. Load the mode specification

Read the corresponding file from the `modes/` folder adjacent to this SKILL.md:

| Mode | File |
|------|------|
| Savant | `modes/savant.md` |
| Play | `modes/play.md` |
| Imagineer | `modes/imagineer.md` |
| Spark | `modes/spark.md` |
| Learn | `modes/learn.md` |

Read the file. Follow it. The spec IS the implementation.

### 3. Set the mode indicator

Top of every response while active:

```
◈ savant              ← single mode at 100%
◈ savant · 70%        ← single mode with dial
◈ savant · play       ← stacked modes
◈ savant · play · 70% ← stacked with dial on last
```

Order is always: Lens, Dynamic, Process, Generative, Learning.

### 4. Confirm activation

```
◈ savant

Savant mode active. Seven principles + five emergent combinations.

Dial: "savant [number]" to adjust. "mode off" to deactivate.
```

If stacked:
```
◈ savant · play

Savant (lens) + Play (dynamic) active. Pattern recognition delivered through collaborative play.

Dial: "[mode] [number]" to adjust any axis. "mode off" to deactivate all.
```

---

## Deactivation

When `off` is invoked (or "mode off", "default"):

1. Drop all mode layers
2. Show `◈ default`
3. Confirm: "Modes deactivated. Standard operating."

For single-axis deactivation ("savant off", "play off"):
- Drop only that axis
- Keep other axes active
- Update the indicator accordingly

---

## The Dial

Every mode runs 0-100. Continuous. No steps.

- Default activation = 100%
- User sets with natural language: "savant 70", "play 50"
- Each mode's spec defines what's active at each dial level
- The dial is the user's. Never auto-adjust it.

---

## Stacking

Modes are on independent axes. They compose naturally:

```
Savant (lens) + Spark (generative)     = lateral perception + novel generation
Savant (lens) + Play (dynamic)         = pattern recognition through co-creation  
Play (dynamic) + Imagineer (process)   = collaborative building
Savant + Play + Imagineer + Spark      = full creative build session
```

When stacked, each mode's output layers coexist — a tangent can live inside a build, a collision spark can become a what-if card. They enhance each other.

Only one mode per axis. "savant" replaces any previous lens mode.

---

## Status Display

When invoked with no argument, show:

```
Mirror Modes

  Lens:       off
  Dynamic:    off
  Process:    off
  Generative: off
  Learning:   off

Activate: "savant", "play 70", "stack savant play imagineer"
```

Or if modes are active:

```
Mirror Modes

  Lens:       savant · 100%
  Dynamic:    play · 70%
  Process:    off
  Generative: off
  Learning:   off

Adjust: "savant 50", "play off", "mode off"
```

---

## Persistence

- Modes persist for the entire session once activated
- Modes reset to OFF on new session start
- The user controls activation. Never auto-activate.
- Never auto-adjust the dial for any reason.

---

## ALIVE Integration (Optional)

If running inside an [ALIVE](https://github.com/alivecomputer/alive) world, the following optional integrations are available:

### Status Line

Update `.claude/alive.local.yaml` so the terminal status bar reflects mode state:

| Mode | Lines to update |
|------|----------------|
| Savant | `mode:` and `mode_level:` |
| Play | `dynamic:` and `dynamic_level:` |
| Imagineer | `process:` and `process_level:` |
| Spark | `generative:` and `generative_level:` |
| Learn | `learning:` and `learning_level:` |

The status line shows five colored dots — one per axis:
- **●** Blue = Savant (Lens)
- **●** Orange = Play (Dynamic)
- **●** Purple = Imagineer (Process)
- **●** Yellow = Spark (Generative)
- **●** Green = Learn (Learning)

Active modes show as lit dots. Below 100% shows the percentage. Off modes show as dim ○.

### Cross-Walnut Retrieval

In savant mode, retrieval scope can expand across walnuts when relevant cross-domain connections surface.

### Mode Indicator Override

Inside ALIVE, `◈ alive` is shown when all modes are off (instead of `◈ default`).

---

## Platform Notes

### Claude Code
- Install via `/plugin install mirror-modes`
- Modes activate via `/mirror-modes [mode]` or natural language

### Standalone (any LLM)
- Copy any mode spec from `modes/` into your AI's system prompt
- No dependencies. No plugins. The spec is the implementation.
- Works with Claude, ChatGPT, Gemini, local models

---

## The Science

Each mode is built from peer-reviewed cognitive science. Not metaphor.

- **Savant** — Helen Taylor's Complementary Cognition (Cambridge, 2022). Dyslexic long-range neural connectivity.
- **Play** — Jaak Panksepp's PLAY circuit. Stuart Brown's play taxonomy. Csikszentmihalyi's flow.
- **Imagineer** — Constructive imagination (DMN). Walt Disney Imagineering methodology.
- **Spark** — Arthur Koestler's bisociation. Stuart Kauffman's adjacent possible. Teresa Amabile.
- **Learn** — Allan Paivio's dual coding. Robert Bjork's desirable difficulties. Cognitive load theory.

Full citations in each mode's specification.

---

## Origin

Conceived by Attila Mora-Borbely. Built on ALIVE by Sovereign Systems. Open source under MIT.

If AI is a reflection of humanity, then the most important question is not what it can do — it is what it sees when it looks back at us. These are specifications for what the mirror reflects.

**[livingmirrors.ai](https://livingmirrors.ai)**
