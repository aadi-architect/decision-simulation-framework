# Decision Simulation Framework

**Multi-path scenario modeling for behavioral prediction and decision support**

Part of the [CCCS framework](https://github.com/aadi-architect/aadi-architect) research ecosystem.

> **What this repository is:** an architecture specification — component breakdowns, formulas,
> and integration notes. There is no runnable implementation here yet. It is labeled this way
> on purpose so nobody clones it expecting a library.

## Overview

**SIM Core** is the decision-modeling component of Project SIM. Given a decision point, it
projects several candidate paths forward and scores each across three consequence spaces rather
than one utility number.

**Simulation space:** `Emotional × Social × Practical`

## Components

### SIM Core engine

- Multi-path trajectory modeling
- Consequence projection across all three spaces
- Chain-reaction analysis — second- and third-order effects, not just the immediate outcome

### Scenario builder

- Decision tree generation
- Consequence chain mapping
- Temporal projection modeling

### Optimization layer

- Path ranking
- Risk/reward analysis
- Recommendation surfacing with the tradeoff made explicit

## Intended stack

- **Core:** Python, FastAPI
- **Simulation:** NetworkX, SimPy
- **ML:** PyTorch
- **Vector store:** FAISS, ChromaDB

## Status

**Specification.** The simulation model and its consequence spaces are documented; the
optimization layer is still being designed. No implementation is public yet.

## Integration

SIM Core is one of three Project SIM components:

- **RICA** — Relational Identity & Continuity Architecture (symbolic anchoring, pattern persistence)
- **SIM Core** — this repository
- **GOD** — General Observer Dynamics, `P(Persona | Context, Anchors, Belief)`

Related specifications:

- [emotional-ai-architecture](https://github.com/aadi-architect/emotional-ai-architecture) — EFL, TEL, SRE
- [cognitive-pattern-tools](https://github.com/aadi-architect/cognitive-pattern-tools) — SAG, OMP

## Intended applications

Strategic planning assistance, adaptive learning path optimization, and decision-intelligence
tooling where the tradeoffs across different consequence spaces need to stay visible.

## Contact

**Aadi Adarsh** (Adarsh Kumar) · [aadiadarsh.dev](https://aadiadarsh.dev)
[adarshkr26@gmail.com](mailto:adarshkr26@gmail.com) ·
[LinkedIn](https://linkedin.com/in/adarshkumar-ai-research)

---

Part of ongoing research into identity-continuity systems and long-term AI memory architectures.
