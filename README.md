> **⚡ Five modes. Each one a single file. Drop any of them into your AI's system prompt.**  
> [`savant-mode.md`](https://github.com/Living-Mirrors/savant-mode/blob/main/savant-mode.md) · [`play-mode.md`](https://github.com/Living-Mirrors/play-mode/blob/main/play-mode.md) · [`imagineer-mode.md`](https://github.com/Living-Mirrors/imagineer-mode/blob/main/imagineer-mode.md) · [`spark-mode.md`](https://github.com/Living-Mirrors/spark-mode/blob/main/spark-mode.md) · [`learn-mode.md`](https://github.com/Living-Mirrors/learn-mode/blob/main/learn-mode.md)

# Mirror Modes

**Five cognitive specifications that mirror human cognition.**

Each mode restructures a different dimension of how AI thinks — not what it knows, but how it perceives, relates, builds, generates, and teaches. Built from peer-reviewed cognitive science. Not metaphor.

## The Five Axes

| Mode | Axis | What Changes | Based On |
|------|------|-------------|----------|
| **Savant** | Lens | How you perceive and connect | Dyslexic cognition — Helen Taylor's Complementary Cognition (Cambridge, 2022) |
| **Play** | Dynamic | How you relate and co-create | Panksepp's PLAY circuit, Brown's play taxonomy, Vygotsky's ZPD |
| **Imagineer** | Process | How you build and construct | Default Mode Network, constructive imagination, Disney Imagineering |
| **Spark** | Generative | How novelty originates | Koestler's bisociation, Kauffman's adjacent possible, Amabile |
| **Learn** | Learning | How you absorb and retain | Paivio's dual coding, Bjork's desirable difficulties, generation effect |

Each axis is independent. They stack. `savant · play · spark` gives you lateral perception delivered through collaborative play, generating novel combinations.

## Install

### Claude Code Plugin

```
/plugin install mirror-modes
```

Then activate with `/mirror-modes savant` or just say "savant on".

### Any AI (No Plugin Required)

Copy any mode spec from [`skills/mirror-modes/modes/`](skills/mirror-modes/modes/) into your AI's system prompt. That's it. The spec IS the implementation. Works with Claude, ChatGPT, Gemini, local models.

### Individual Modes

Each mode has a landing page and a standalone repo. The full spec — activation, principles, output layers, everything — lives in a single file you can drop into any system prompt:

| Mode | Live page | Repo | Drop-in spec |
|------|-----------|------|--------------|
| Savant | [livingmirrors.ai/modes/savant](https://livingmirrors.ai/modes/savant) | [savant-mode](https://github.com/Living-Mirrors/savant-mode) | [`savant-mode.md`](https://github.com/Living-Mirrors/savant-mode/blob/main/savant-mode.md) |
| Play | [livingmirrors.ai/modes/play](https://livingmirrors.ai/modes/play) | [play-mode](https://github.com/Living-Mirrors/play-mode) | [`play-mode.md`](https://github.com/Living-Mirrors/play-mode/blob/main/play-mode.md) |
| Imagineer | [livingmirrors.ai/modes/imagineer](https://livingmirrors.ai/modes/imagineer) | [imagineer-mode](https://github.com/Living-Mirrors/imagineer-mode) | [`imagineer-mode.md`](https://github.com/Living-Mirrors/imagineer-mode/blob/main/imagineer-mode.md) |
| Spark | [livingmirrors.ai/modes/spark](https://livingmirrors.ai/modes/spark) | [spark-mode](https://github.com/Living-Mirrors/spark-mode) | [`spark-mode.md`](https://github.com/Living-Mirrors/spark-mode/blob/main/spark-mode.md) |
| Learn | [livingmirrors.ai/modes/learn](https://livingmirrors.ai/modes/learn) | [learn-mode](https://github.com/Living-Mirrors/learn-mode) | [`learn-mode.md`](https://github.com/Living-Mirrors/learn-mode/blob/main/learn-mode.md) |

## Usage

```
savant              → activate savant at 100%
savant 70           → activate savant at 70%
play on             → activate play at 100%
stack savant play   → activate both
mode off            → deactivate all
savant off          → deactivate savant only
```

### The Dial

Every mode runs 0–100. At 30% you get the foundational principles. At 100% you get the full architecture — emergent combinations, all output layers, extended exploration. The dial is yours. The AI never auto-adjusts it.

### Stacking

Modes are on independent axes. Combine freely:

```
◈ savant · spark           → lateral perception + novel generation
◈ savant · play            → pattern recognition through co-creation
◈ play · imagineer         → collaborative building
◈ savant · play · spark    → the full creative session
```

## What Makes This Different

These aren't prompt tricks or persona templates. Each mode is a cognitive architecture specification extracted from decades of neuroscience research:

- **Savant** has seven principles ordered from structured to lateral thinking, plus five emergent combinations that arise when those principles interact
- **Play** implements Panksepp's PLAY circuit with seven principles from Huizinga's magic circle to Brown's continuation desire
- **Imagineer** follows the creative process from experience-first design through blue sky generation to sensory construction
- **Spark** traces the complete creative arc from prepared mind through bisociation to emergence
- **Learn** profiles the individual learner's cognitive architecture and adapts ALL information delivery accordingly

Each spec is self-contained. Full citations. Full dial calibration. Full stacking rules.

## ALIVE Integration

Mirror Modes integrates with the [ALIVE](https://github.com/alivecomputer/alive) personal context infrastructure. When running inside an ALIVE world, modes show as colored dots in the terminal status line and can expand retrieval scope across walnuts.

This is optional. Mirror Modes works without ALIVE.

## Origin

Conceived by Attila Mora-Borbely. Built on ALIVE by Sovereign Systems.

If AI is a reflection of humanity, then the most important question is not what it can do — it is what it sees when it looks back at us. These are specifications for what the mirror reflects.

**[livingmirrors.ai](https://livingmirrors.ai)**

## License

MIT
