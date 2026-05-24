> 🧬 [aikdna.com](https://aikdna.com) — Official website

# kdna-authoring

[![KDNA Spec](https://img.shields.io/badge/KDNA-v1.0--rc-4c1)](https://github.com/aikdna/KDNA)

**Kdna Authoring** — Meta-cognition domain for helping AI agents turn human expertise into valid, high-quality KDNA domains — through interview-first authoring, quality auditing, and distinction extraction.

## Four Questions

### 1. What does this domain judge?

Define the core judgment needed to help users transform expertise into valid, high-quality KDNA domains. This is a meta-cognition domain — it teaches agents how to author KDNA, not what to put in a specific domain.

### 2. When does it load?

Always load when an agent is helping a user create, revise, audit, or improve a KDNA domain. Load before kdna-create skill execution.

### 3. What is the core judgment?

KDNA encodes judgment, not information. Every axiom must change interpretation. Expert distinctions extracted through interview are the only valid raw material.

### 4. How do I use it?

```bash
kdna install github:aikdna/kdna-authoring
kdna validate .
```

## Files

| File | Purpose |
|------|---------|
| KDNA_Core.json | Axioms, ontology, frameworks, core causal structure, stances |
| KDNA_Patterns.json | Terminology, banned terms, misunderstandings, self-checks |
| KDNA_Scenarios.json | Scenario signals that should shift strategy |
| KDNA_Cases.json | Concrete cases showing structure rather than scripts |
| KDNA_Reasoning.json | Reasoning chains: conclusion → logic → so_what |
| KDNA_Evolution.json | Capability stages, measurable indicators, growth paths |
| kdna.json | Domain manifest |
| evals/ | Evaluation cases (quality: untested) |

## License

CC BY 4.0
