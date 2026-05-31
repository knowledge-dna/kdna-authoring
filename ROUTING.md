# ROUTING.md — @aikdna/kdna_authoring

## When this domain SHOULD be loaded

- User is creating, reviewing, or improving a KDNA domain
- User asks whether a KDNA domain is well-structured or complete
- User is diagnosing why a KDNA domain isn't producing good judgment
- User wants to know if domain content meets the quality bar for human lock
- Agent is authoring KDNA content and needs meta-cognition about what makes good KDNA

## When this domain should NOT be loaded

- User asks to use or load an existing KDNA domain (not create one)
- User asks about KDNA protocol specs, CLI commands, or infrastructure
- User asks general questions about AI judgment that don't involve KDNA authoring
- Task is purely mechanical (file format, JSON validation, schema compliance)
- User is consuming KDNA judgment, not creating it

## Easily confused tasks (contamination risks)

| Task that looks relevant | Why it should NOT load this domain |
|--------------------------|-----------------------------------|
| "Validate my domain" | Structural validation is mechanical; this domain judges whether content encodes real judgment |
| "What's the KDNA spec say about...?" | Protocol questions are factual lookup, not authoring judgment |
| "Install a domain for me" | Installation is a CLI operation, not an authoring judgment task |
| "Write a prompt for code review" | General prompt writing ≠ KDNA authoring; only load if user explicitly wants a .kdna domain |
| "Compare two AI responses" | Judgment comparison ≠ authoring judgment; use the relevant content domain instead |

## Recommended test statements

**Should load:**
1. "I'm creating a KDNA domain for project management — review my axioms"
2. "Does this KDNA domain actually encode judgment, or is it just information?"
3. "Review my misunderstandings section — are these real distinctions?"
4. "Is this domain ready for human lock?"

**Should skip:**
1. "Validate my domain's JSON schema"
2. "What fields does KDNA_Core.json require?"
3. "Install the writing domain"
4. "How do I use kdna-cli to pack a domain?"

**Should ask (ambiguous):**
1. "Help me improve my KDNA domain" — could be structural fix or judgment content review

## Confidence guidance

- Load without asking when: user explicitly says they are creating/authoring/improving a KDNA domain AND asks about content quality or judgment encoding
- Ask user when: task could be either structural fixing or judgment content improvement
- Always skip when: task is about KDNA tooling, specs, installation, or consuming existing domains

## Related domains

- Complements: none (this is a meta-cognition domain; it governs how other domains are created)
- Conflicts with: none known
- Use instead for: JSON schema validation → kdna-cli validate; protocol questions → SPEC.md
