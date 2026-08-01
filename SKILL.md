---
name: human-prose
description: Sentence-level readability rules for any prose a human will read — file comments, docstrings, module docs, commit messages, PR descriptions, chat explanations. Use when writing or rewriting such prose, when the user says text is dense, overwhelming, machine-written, or a long block of text, or when another skill's output needs a readability pass. Canonical home of this rule set; other skills point here rather than duplicating it.
---

# Human prose

Write for a reader who processes one clause at a time. Each rule below
removes a documented processing cost. The evidence base with full
citations is `references/evidence.md`; load it only when a rule is
questioned or amended, or when a full citation must be quoted.

## The rules

1. **One idea per sentence, kept short.** Comprehension falls as sentence
   length rises (Flesch 1948). Split rather than subordinate.
2. **No mid-sentence interruptions.** An em-dash aside or a nested
   parenthetical suspends a clause the reader must hold open (Gibson
   1998). Write a second sentence instead. A short parenthetical label
   (like this one) is fine; a clause-length intrusion is not.
3. **Active voice; verbs over nominalizations.** Passives verify slower
   than actives (Gough 1965). Nominalized prose reads worse than its
   active-verb form (Coleman 1964).
4. **Given before new.** Open each sentence from material the reader
   already has, then add the new (Haviland & Clark 1974). No inverted
   openings ("Nor was X a one-off").
5. **No decorative emphasis.** Emphasis works by selectivity (Schneider
   et al. 2018). Flourishes are seductive details, and those measurably
   hurt learning (Rey 2012). One signal per scope, chosen deliberately.
6. **Plain register.** Jargon appears at most once, as a parenthetical
   label on the plain phrase it names. (User rule, 2026-08-01: plain language.)

## The pass

Apply the rules as a dedicated pass after the content is complete, not
while drafting. Keep verbatim material untouched: quotes, compiler
error text, signatures, citations. In Lean files, verify afterwards
that the diagnostic set is unchanged; in Lean files all commentary goes
in `/- ... -/` blocks, never `--` line comments.
