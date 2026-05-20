> 🧬 [aikdna.com](https://aikdna.com) — Official website

# kdna-authoring

[![KDNA Spec](https://img.shields.io/badge/KDNA-v0.4-4c1)](https://github.com/knowledge-dna/KDNA)

**KDNA Authoring** — A meta-cognition domain that teaches AI agents how to help humans create high-quality KDNA domains through interview-first authoring, quality auditing, and distinction extraction.

## Core Insight

KDNA encodes judgment, not information. Every axiom must change interpretation. Expert distinctions extracted through interview are the only valid raw material.

## Scope

This domain helps AI agents judge HOW to author a KDNA domain — what questions to ask, what content is valid judgment vs hollow material, and how to audit quality. It is designed for agents running kdna-create skill, and for users who want to encode their expertise.

## Out of Scope

This domain is NOT a KDNA template library. It is NOT a prompt for generating KDNA automatically. It is NOT a questionnaire or form-filling guide. It encodes the JUDGMENT agents need to conduct effective authoring sessions — not the mechanical steps of writing JSON.

## Install

```bash
kdna install github:knowledge-dna/kdna-authoring
```

## Files

| File | Purpose |
|------|---------|
| KDNA_Core.json | Axioms, ontology, frameworks, core causal structure, stances |
| KDNA_Patterns.json | Terminology, banned terms, misunderstandings, self-checks |
| KDNA_Scenarios.json | 5 authoring scenarios: stories, frameworks, documents, drafts, skills |
| KDNA_Cases.json | 3 cases: expert story→KDNA, skill→KDNA, hollow KDNA audit |
| KDNA_Reasoning.json | 4 reasoning chains explaining why each rule matters |
| KDNA_Evolution.json | 4 capability stages + 5 measurable indicators |
| kdna.json | Domain manifest |

## Validate

```bash
kdna validate .
```

## License

CC BY 4.0
