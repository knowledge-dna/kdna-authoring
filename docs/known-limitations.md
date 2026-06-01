# @aikdna/kdna_authoring — Known Limitations

## Domain Scope Boundaries

This domain provides **meta-cognition for KDNA authoring**. It does NOT replace:

- **Domain expertise** — the author must still bring real judgment, not just process
- **Studio Core** — this KDNA guides authoring decisions; Studio Core enforces the technical contract
- **Human judgment** — AI proposes candidates; only humans confirm judgment

## Known Failure Modes

### 1. Treating information compression as judgment extraction
**When it happens:** Agent reads content, summarizes key points, and presents them as KDNA axioms. This produces a content outline in KDNA format — not judgment. The test: can any axiom be removed and the remaining ones still work? If yes, it's information, not judgment.
**Mitigation:** Every axiom must change interpretation. Test: "If I remove this axiom, would the agent produce the same output?"

### 2. Defaulting to interview-only across all contexts
**When it happens:** Author has rich existing content but the agent insists on an interview, missing the distillation-first path entirely. The author gets frustrated because they're asked to re-describe what they've already written.
**Mitigation:** Check: does the author have existing content that encodes their judgment? If yes, propose distillation-first.

### 3. Creating hollow KDNA — axioms with no behavioral consequence
**When it happens:** Agent produces axioms like "quality matters" or "be thorough" — universally true statements that don't change any agent behavior. These pass structure validation but fail the behavioral test.
**Mitigation:** Every axiom must: (a) rule something out, (b) prioritize one concern over another, or (c) classify a situation differently than an unguided agent would.

### 4. Accepting broad-scope KDNA that should be split
**When it happens:** Agent creates one large KDNA covering "software engineering" instead of splitting into "code review," "architecture decisions," and "testing strategy." The KDNA becomes too broad to be useful — applies to everything, shapes nothing.
**Mitigation:** One `.kdna` = one scoped judgment domain. If the domain covers multiple judgment lenses, split them and compose via a KDNA Cluster.

### 5. Skipping Human Lock verification steps
**When it happens:** Agent proposes judgment cards and the author approves them without verifying `applies_when`, `does_not_apply_when`, and `failure_risk`. The resulting KDNA loads on wrong tasks or produces wrong outputs.
**Mitigation:** Human Lock must confirm at minimum: applies_when, does_not_apply_when, failure_risk.

## When NOT to use this KDNA

- User is creating content that is purely informational (knowledge base, FAQ)
- User is writing prompts or system instructions (not KDNA)
- User is documenting procedural workflows (not judgment frameworks)
- User explicitly declines the KDNA authoring framework

## Eval Coverage

- 10 standardized eval cases in `evals/`
- Covers: axiom validity tests, hollow KDNA detection, misunderstanding patterns, authoring path selection

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 0.7.0 | 2026-05 | Current release |
