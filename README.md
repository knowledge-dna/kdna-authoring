> 🧬 [aikdna.com](https://aikdna.com) — Official website

# @aikdna/kdna_authoring

[![KDNA Spec](https://img.shields.io/badge/KDNA-v1.0--rc-4c1)](https://github.com/aikdna/KDNA)

**KDNA authoring judgment** — meta-cognition domain for helping AI agents turn human expertise into valid, high-quality KDNA domains.

## What this KDNA changes

**Before loading this KDNA, an agent tends to:**
- Treat domain authoring as information gathering
- Add general knowledge without extracting expert distinctions

**After loading this KDNA, an agent will judge:**
- Is this encoding judgment, not information?
- Does every axiom change interpretation?
- Are expert distinctions extracted through interview the only valid raw material?
- Is the domain following interview-first authoring?

## This KDNA is for

- Helping users create, revise, audit, or improve a KDNA domain
- Interview-first authoring workflows
- Quality auditing and distinction extraction

## This KDNA is not for

- General knowledge base creation
- Prompt engineering
- Domain content that is not KDNA-structured

## Core judgment

KDNA encodes judgment, not information. Every axiom must change interpretation. Expert distinctions extracted through interview are the only valid raw material.

## Self-checks

- Is this encoding judgment, not just information?
- Does every axiom change how an agent would interpret a situation?
- Was this extracted from expert interview or just general knowledge?
- Are the boundaries clear enough to refuse loading on wrong tasks?

## Install

```bash
kdna install @aikdna/kdna_authoring
kdna dev validate .
```

## Files

- `KDNA_Core.json` — Axioms, ontology, frameworks, causal structure, stances
- `KDNA_Patterns.json` — Terminology, banned terms, misunderstandings, self-checks
- `KDNA_Scenarios.json` — Scenario signals that shift strategy
- `KDNA_Cases.json` — Concrete cases showing judgment structure
- `KDNA_Reasoning.json` — Reasoning chains: conclusion → logic → action
- `KDNA_Evolution.json` — Capability stages, measurable indicators, growth paths
- `evals/` — Evaluation cases (quality: untested)
- `kdna.json` — Domain manifest

## License

CC BY 4.0
