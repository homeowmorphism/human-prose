# Human prose — evidence base

Load policy: not needed to apply the rules. `SKILL.md` is operationally
self-sufficient; load this file when a rule is questioned or amended, or
when a full citation must be quoted.

History: distilled 2026-08-01 from user feedback in the
`Group.Presentation` project. The sentence rules came from a request to rewrite the docstrings, which were hard to read (on `scratch_field_vs_parameter.lean`). The register rule came
from an earlier instruction in the same project: plain language.
The rules first lived in the mathlib-definition skill (renamed
`mathlib-api` on 2026-08-02;
`references/example-sheet-evidence.md` §Prose readability) and moved
here the same day so that any skill, or no skill, can apply them.

## Rule → finding

- **Short sentences, one idea each.** Comprehension falls as sentence
  length rises; sentence length is one of the two variables in the
  classical readability formulas (Flesch 1948).
- **No mid-sentence interruptions.** An em-dash aside or a nested
  parenthetical is a center-embedded constituent: the reader holds the
  suspended clause in working memory for the length of the intrusion
  (Gibson 1998). Prefer a second sentence.
- **Active voice; verbs over nominalizations.** Passives take longer to
  verify than actives (Gough 1965); prose rewritten from nominalizations
  into active verbs is more comprehensible (Coleman 1964).
- **Given before new.** Sentences integrate faster when they open from
  already-established material (Haviland & Clark 1974). This also rules
  out inverted openings.
- **No decorative emphasis.** Signaling works by selectivity (Schneider
  et al. 2018), and interesting-but-irrelevant flourishes measurably
  hurt learning (the seductive-detail effect: Rey 2012).
- **Plain register.** User rule; no external citation claimed. Analogy
  and plain phrasing first, each technical term at most once as a label.

## Bibliography

Verification status: Coleman 1964 and Rey 2012 were verified against
publisher/index records on 2026-08-01. Schneider et al. 2018 was
verified 2026-07-31 for the mathlib-definition bibliography. Flesch,
Gough, Gibson, and Haviland & Clark are cited from standard
bibliographic knowledge; re-verify before quoting externally.

- Flesch, R. (1948). A new readability yardstick. *Journal of Applied
  Psychology*, 32(3), 221–233. Reading ease as a function of sentence
  length and word length.
- Coleman, E. B. (1964). The comprehensibility of several grammatical
  transformations. *Journal of Applied Psychology*, 48(3), 186–190. Four
  experiments; active-verb transforms beat nominalizations and passives.
- Gough, P. B. (1965). Grammatical transformations and speed of
  understanding. *Journal of Verbal Learning and Verbal Behavior*, 4(2),
  107–111. Passives and negatives take longer to verify than actives.
- Haviland, S. E., & Clark, H. H. (1974). What's new? Acquiring new
  information as a process in comprehension. *Journal of Verbal Learning
  and Verbal Behavior*, 13(5), 512–521. Sentences are understood faster
  when given information precedes new.
- Gibson, E. (1998). Linguistic complexity: Locality of syntactic
  dependencies. *Cognition*, 68(1), 1–76. Processing cost grows with the
  distance over which an incomplete dependency is held open.
- Schneider, S., Beege, M., Nebel, S., & Rey, G. D. (2018). A
  meta-analysis of how signaling affects learning with media.
  *Educational Research Review*, 23, 1–24. doi:10.1016/j.edurev.2017.11.001.
  Cueing the relevant material or its organization reliably improves
  retention and transfer.
- Rey, G. D. (2012). A review of research and a meta-analysis of the
  seductive detail effect. *Educational Research Review*, 7(3), 216–237.
  doi:10.1016/j.edurev.2012.05.003. Interesting but irrelevant additions
  reliably reduce retention and transfer.
