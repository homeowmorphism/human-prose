# human-prose

A [Claude Code](https://claude.com/claude-code) skill holding
sentence-level readability rules for prose a human will read: file
comments, docstrings, module docs, commit messages, PR descriptions,
chat explanations. Each rule removes a documented processing cost, and
each is pinned to the psycholinguistics and multimedia-learning
literature. Domain-general: the prose can live in a Lean file, a Python
docstring, or a design memo.

Distilled (2026-08-01) from editing sessions on a Lean 4 / mathlib
project, where dense machine-written comments were reported as
overwhelming to read. The rules first lived inside
the [mathlib-api](https://github.com/homeowmorphism/mathlib-api)
skill (then named `mathlib-definition`) and were refactored out the same
day, so that any skill can apply them.
[adaptive-teacher](https://github.com/homeowmorphism/adaptive-teacher)
and mathlib-api both defer their prose style here.

## The rules

1. One idea per sentence, kept short (Flesch 1948).
2. No mid-sentence interruptions. An em-dash aside or a nested
   parenthetical suspends a clause the reader must hold open
   (Gibson 1998). Write a second sentence instead.
3. Active voice; verbs over nominalizations (Gough 1965; Coleman 1964).
4. Given before new: open each sentence from material the reader
   already has (Haviland & Clark 1974).
5. No decorative emphasis. Emphasis works by selectivity (Schneider et
   al. 2018), and flourishes are seductive details (Rey 2012).
6. Plain register: jargon at most once, as a parenthetical label on the
   plain phrase it names.

The rules are applied as a dedicated pass after the content is
complete. Verbatim material (quotes, compiler errors, signatures,
citations) stays untouched.

## Repository layout

```
SKILL.md               entry point, self-sufficient: the rules and
                       the pass
references/
  evidence.md          on-demand evidence base: rule → finding mapping,
                       history, bibliography with per-entry
                       verification status
```

## Installation

As a personal skill (available in all projects), clone into
`~/.claude/skills/human-prose`. As a project skill, clone into
`.claude/skills/human-prose` inside the project instead. Invoke it
explicitly with `/human-prose`, or let Claude pick it up from the
skill description when prose needs a readability pass.

## Citation

Author: Hang Lu Su ([homeowmorphism](https://github.com/homeowmorphism)).

Please cite this skill if you use it in published work, ship it inside a
tool, or build a derivative of it. GitHub's "Cite this repository" button
reads [CITATION.cff](CITATION.cff) and gives you BibTeX or APA. In plain
text:

> Su, Hang Lu. *human-prose: a Claude Code skill for sentence-level
> readability.* https://github.com/homeowmorphism/human-prose

## License

[Apache License 2.0](LICENSE.md): free to use, modify, and share, for
any purpose, with an explicit patent grant. Keep [LICENSE.md](LICENSE.md)
and [NOTICE](NOTICE) with any redistribution.
