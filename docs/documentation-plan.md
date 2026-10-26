# Documentation plan

This repo shows the finished site and how it was built with AI tools. The documentation keeps that process visible and short enough to read in two minutes.

## What gets documented

| What | Where |
| ----- | ----- |
| Build sessions: what was done, prompts used, results | `docs/build-log.md` |
| Decisions: any choice with trade-offs | `docs/decisions/`, one file per decision |
| Reusable prompts | `prompts/`, one file per prompt |
| Case studies | `case-studies/`, under 250 words each |

## When

- **End of every session:** a dated build log entry.
- **When a choice has trade-offs:** a decision record, written at the time.
- **When a prompt is worth reusing:** saved to `prompts/` from the template.

## Commit messages

`type: short description`, in lower case, under 60 characters.

| Type | Use for |
| ----- | ----- |
| `build` | Site structure, code and styling |
| `content` | Copy on the site and case studies |
| `docs` | Build log, decisions, prompts, this plan |
| `fix` | Corrections to anything above |

Example: `content: update case study 2 situation`

## Never in the repo

Nothing confidential or private: no client names, internal financials, employer detail, or working files (`advert.md`, `cv.md`, `notes.md`).

## Templates

Leave out any line that would be empty.

**Build log entry**
```
## YYYY-MM-DD: [session goal]
**Built:** [what changed]
**Prompt used:** [link to prompts/ file]
**Decision:** [link to decision record, if any]
**What worked:** [one line]
**What I changed:** [one line]
**Time spent:** [minutes]
```

**Decision record** (`docs/decisions/NNN-short-name.md`)
```
# [Number]: [Decision]
**Date:** [date]
**Options considered:** [A, B]
**Chosen:** [A]
**Why:** [one or two sentences]
**Trade-off accepted:** [one sentence]
```

**Prompt** (`prompts/short-name.md`)
```
# [Prompt name]
**Purpose:** [what it produces]
**Inputs:** [files or context needed]
**Prompt:** [the prompt, in a code block]
**Notes:** [what to edit before reuse]
```

**Case study** (`case-studies/short-name.md`)
```
# [Title]
**Context:** [company type, customer type, scale]
**Problem:** [one or two sentences]
**What I did:** [3 to 5 bullets]
**Result:** [metric, or what changed, who adopted it and what decision it enabled]
**What I would do differently:** [one sentence]
**Relevance to this role:** [one sentence]
```
