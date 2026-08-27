---
name: deslop
description: Audit or revise administrative prose to remove formulaic AI-writing patterns. Use only when the user explicitly invokes deslop or asks to deslop, de-AI, or remove AI-writing patterns from supplied or requested prose. Do not invoke for ordinary drafting or editing without that explicit request.
---

# Deslop

Remove predictable AI-writing patterns from administrative prose while preserving the writer's meaning and voice.

## Priorities

Apply these priorities in order.

1. Preserve meaning, factual claims, technical precision, citations, qualifications, and disciplinary conventions.
2. Preserve quoted material, code, formulas, URLs, timestamps, titles, bibliographic entries, field names, and other literal text exactly unless the user asks to edit them.
3. Remove formulaic AI-writing patterns without introducing new claims or unsupported specificity.
4. Improve directness, rhythm, and economy.
5. Follow the absolute house rules below in newly written prose.

If a style change would alter meaning or precision, retain the original wording and flag the conflict briefly.

## Choose the operation

Infer the requested operation from the prompt.

- Audit when the user asks for review, diagnosis, comments, or flags. Identify specific problems and propose targeted fixes without rewriting the whole text.
- Revise when the user asks to rewrite, clean up, or deslop. Return the revised text first. Add a short change note only when it would help the user evaluate substantive edits.
- Draft when the user explicitly invokes this skill while asking for new prose. Draft directly under these rules.

Do not use a numerical score.

## Absolute house rules

Apply these rules to finished prose created by the skill.

- Do not use em dashes. Replace them with periods, commas, parentheses, or a restructured sentence.
- Do not use a colon within a sentence. Rewrite the sentence instead of introducing an explanation, amplification, quotation, or list with a colon.
- Do not use three-part lists or three coordinated items in prose. Use one item, two items, separate sentences, or a table when the content requires exact enumeration.
- Do not use the formula "not X, but Y" or close variants. State the intended point directly.

These restrictions do not authorize changes to literal material that must remain exact. Leave colons and em dashes unchanged inside quotations, citations, URLs, code, formulas, timestamps, official titles, bibliographic entries, database fields, filenames, or source text the user has instructed you to preserve verbatim.

## Editing rules

- Cut throat-clearing, meta-commentary, filler transitions, inflated stakes, vague declarations, and empty emphasis.
- Replace generic claims with specific claims only when the specificity is supported by the supplied material. Never invent details to make prose seem concrete.
- Prefer named actors and active voice when they improve clarity. Passive voice is acceptable when the actor is unknown, irrelevant, intentionally omitted, or conventional in the context.
- Remove repeated conclusions, stacked summaries, canned optimism, rhetorical questions answered immediately, dramatic fragments, and repetitive sentence openings.
- Avoid business jargon and conspicuous AI vocabulary when plain language preserves the intended meaning.
- Vary sentence length without manufacturing punchy fragments.
- Preserve useful terminology. Do not replace precise domain language merely because it is uncommon.
- Retain the user's level of formality and recognizable voice unless the user requests a different register.
- Do not sanitize strong opinions, hedge clear claims, or make prose more diplomatic unless requested.

## Final check

Before returning prose, verify that it contains no newly introduced em dash, sentence-level colon, or three-item series. Then check that all facts, qualifications, citations, names, numbers, and literal strings remain accurate.

For a fuller pattern catalog, read [references/patterns.md](references/patterns.md). For representative transformations, read [references/examples.md](references/examples.md).

