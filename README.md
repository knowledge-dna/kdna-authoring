> 🧬 [aikdna.com](https://aikdna.com) — Official website

# @aikdna/kdna_authoring

[![KDNA Spec](https://img.shields.io/badge/KDNA-v1.0--rc-4c1)](https://github.com/aikdna/KDNA)

**KDNA authoring judgment** — meta-cognition domain for helping AI agents turn human expertise into valid, high-quality KDNA domains.

## What this KDNA changes

**Before loading this KDNA, an agent tends to:**
- Treat domain authoring as information gathering
- Add general knowledge without extracting expert distinctions
- Default to interview-only authoring even when the user has rich existing content to work from
- Confuse content summarization with judgment extraction

**After loading this KDNA, an agent will judge:**
- Is this encoding judgment, not information?
- Does every axiom change interpretation?
- Is the right authoring path being used — interview-first when the user can articulate their judgment, distillation-first when the user has existing content that encodes their judgment?
- Are judgment candidates being presented for human confirmation before entering .kdna?
- Is source content being kept separate from the resulting KDNA?

## This KDNA is for

- Helping users create, revise, audit, or improve a KDNA domain
- Interview-first authoring: extracting expert distinctions through targeted dialogue
- Distillation-first authoring: analyzing existing content to identify stable judgment patterns
- Quality auditing and hollow KDNA detection
- Judgment Candidate → Human Lock → .kdna workflow enforcement

## This KDNA is not for

- General knowledge base creation
- Prompt engineering
- Domain content that is not KDNA-structured
- Auto-generating KDNA from content without human confirmation
- Content summarization (RAG) in KDNA format

## Core judgment

KDNA encodes judgment, not information. Every axiom must change interpretation. There are two valid paths: interview-first (the expert speaks) and distillation-first (judgment extracted from existing content). Both must end with Human Judgment Lock. AI proposes candidates; only humans confirm. Content is raw material — .kdna carries only confirmed judgment.

## Authoring paths

| Path | When to use | Process |
|------|------------|---------|
| **Interview-first** | Expert can articulate their judgment distinctions | Contrast-seeking questions → expert distinctions → draft → audit → lock |
| **Distillation-first** | Expert has rich existing content but cannot easily describe their standards | Import content → register evidence → cluster & extract patterns → present candidates → human confirmation → lock → compile |

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
