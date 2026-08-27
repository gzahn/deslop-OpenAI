# Deslop for ChatGPT and Codex

### This is adapted from the [deslop claude skill](https://github.com/stephenturner/skill-deslop) by Stephen Turner

Deslop is an explicitly invoked writing skill for auditing or revising administrative prose. It removes formulaic AI-writing patterns while preserving meaning, technical precision, citations, literal text, and disciplinary conventions.

It is meant to clean up text that you shouldn't be writing anyway, *e.g.*, the narrative portion of an annual review, an executive summary of the monthly Committee to Form Committees meeting, or the self-reflection portion of the annual Conflict of Interest training quiz.

This repository contains both the skill and its plugin wrapper. The plugin has no connector, account, network, or external-service dependencies.

## Use

In ChatGPT, select `@deslop` and provide the text or drafting request.

In Codex CLI or an IDE extension, use `$deslop` or select it from `/skills`.

Example prompts

```text
@deslop Audit this email for AI-writing patterns. Do not rewrite it yet.
```

```text
$deslop Revise this administrative memo conservatively. Preserve every fact, qualification, citation, and required phrase.
```

## Behavior

The skill is explicit-only. It will not activate for ordinary drafting or editing unless the user invokes it or directly asks to deslop or remove AI-writing patterns.

Newly written prose follows three absolute house rules.

- No em dashes
- No sentence-level colons
- No three-item series
- No formulaic negative pivots

Literal text remains unchanged when accuracy requires it. This includes quotations, code, formulas, URLs, timestamps, official titles, bibliographic entries, database fields, and filenames.

## Install and distribute

Upload the contents of this repository to GitHub without adding an extra enclosing directory. The repository root should contain `.codex-plugin`, `skills`, `README.md`, `NOTICE.md`, and `LICENSE`.

Use the repository as a plugin source when installing or sharing through ChatGPT or Codex. For local skill-only testing in Codex, copy `skills/deslop` into `$HOME/.agents/skills/deslop` or a repository's `.agents/skills/deslop` directory.

Restart Codex if a newly installed local skill does not appear.

## License and source

MIT licensed. This adaptation is based on Stephen D. Turner's `skill-deslop` project. See `NOTICE.md` for attribution.
