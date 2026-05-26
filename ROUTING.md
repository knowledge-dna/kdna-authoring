# ROUTING.md — @aikdna/writing

## When this domain SHOULD be loaded

- User asks to review, improve, or diagnose written content (article, blog post, proposal, essay)
- User asks whether a piece of writing is good, effective, or persuasive
- User submits a draft and wants judgment on structure, argument, or evidence quality
- Content feels "weak" but the user can't articulate why

## When this domain should NOT be loaded

- User explicitly asks for grammar check or spelling correction only
- User asks for translation or formatting
- User asks to generate new content from scratch (creation, not judgment)
- User asks for copy-editing or line-level polishing without structural diagnosis
- Task is purely mechanical (word count, file conversion)

## Easily confused tasks (contamination risks)

| Task that looks relevant | Why it should NOT load this domain |
|--------------------------|-----------------------------------|
| "Polish my writing" | Surface polishing ≠ structural diagnosis; user likely wants language edits |
| "Translate this to Chinese" | Translation is mechanical, not judgment |
| "Write a blog post about X" | Generation is creation, not judgment; load only if user asks to review after writing |
| "Fix my grammar" | Grammar is mechanical; this domain diagnoses argument structure |
| "Make this sound smarter" | Tone adjustment without structural diagnosis = surface work |

## Recommended test statements

**Should load:**
1. "Review this article and tell me if the argument holds up"
2. "Is this blog post ready to publish?"
3. "My draft feels weak but I don't know why — can you diagnose it?"
4. "Does this opening paragraph hook the reader?"

**Should skip:**
1. "Fix the grammar in this paragraph"
2. "Translate this article into Chinese"
3. "Format this document for web publishing"
4. "How many words is this article?"

**Should ask (ambiguous):**
1. "Help me improve this article" — could be structural diagnosis or line-level polish

## Confidence guidance

- Load without asking when: user explicitly asks for review/diagnosis/critique AND task involves structure/argument/evidence judgment
- Ask user when: task could be either structural diagnosis or surface polish (e.g. "improve this")
- Always skip when: task is mechanical, generative, or language-only

## Related domains

- Complements: @aikdna/agent_safety (always load as constraint for irreversible publishing actions)
- Conflicts with: none known
- Use instead for: line-level copy editing → prompt without KDNA
