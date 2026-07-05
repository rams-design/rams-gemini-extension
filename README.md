# Rams — Design Review for Gemini CLI

Accessibility (WCAG 2.1) and visual design review for UI code, with concrete
fixes. Made by [rams.ai](https://www.rams.ai/?utm_source=skill&utm_medium=gemini-extension).

## Install

```bash
gemini extensions install https://github.com/rams-design/rams-gemini-extension
```

(Install format per the [Gemini CLI extensions docs](https://github.com/google-gemini/gemini-cli/blob/main/docs/extensions/index.md).)

## Use

Run `/rams path/to/Component.tsx`, or ask for a review naturally ("review this
component for design issues"). The review covers accessibility (alt text,
labels, keyboard access, focus, contrast, touch targets) and visual design
(spacing, typography, color, component states), each finding with a fix.

The extension ships the same review two ways: a `/rams` custom command and a
`rams` agent skill, so it works whether you invoke it or the model reaches for it.

## Canonical source

The review content is maintained at
[rams.ai/rams.md](https://rams.ai/rams.md) — that file is canonical. A nightly
workflow syncs this repo to it, so the extension never drifts.

## The full engine

This extension runs locally as a heuristic review. The hosted engine at
[rams.ai](https://www.rams.ai/?utm_source=skill&utm_medium=gemini-extension)
reviews every pull request with 119 scored rules, verified re-reviews, and
one-click fix suggestions.

MIT licensed.
