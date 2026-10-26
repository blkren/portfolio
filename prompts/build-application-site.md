# Build an application site

**Purpose:** A role-specific portfolio page that maps a job advert to evidence, with a claims check, a commit and a build log entry.

**Inputs:** `advert.md`, `cv.md`, `evidence-brief.md`, and `cv.pdf` if available.

**Prompt:**

```
You are helping me build a portfolio site that I will link in a job application for a Customer Success Manager role at Juicebox (AI recruiting software, PLG, hypergrowth, London on-site). The site's single job is to show, quickly and with evidence, why I match their advert.

INPUTS
- advert.md: the full job advert
- cv.md: my CV as text
- cv.pdf, if present: copy it to assets/cv.pdf as the downloadable CV; if it is missing, leave the CV link as a placeholder
- The evidence brief at the end of this prompt

RULES
- UK English. No em dashes. Confident but grounded tone, no hype words ("passionate", "rockstar", "world-class").
- Frame achievements around customer and business outcomes, not personal ownership.
- Never invent or round up a number. If a fact is missing or marked [confirm], ask me before writing it.
- Where an outcome cannot be measured, say what changed, who adopted it and what decision it enabled.
- No client names, internal financials or confidential detail from my current employer. Describe it as "a UK professional services compliance business serving 3,000 schools and trusts".

PAGE STRUCTURE (/juicebox/index.html)
1. Hero: one-line positioning for this role, my name, links to CV (PDF), LinkedIn and email.
2. "Your advert, my evidence": a table with three columns: what Juicebox asks for, what I have done, the result. One row per requirement in the brief.
3. Three short case studies (situation, what I did, result, 120 words max each).
4. "My first 90 days at Juicebox": learn the product and customers, run success plans and QBRs, then improve the playbook. Keep it to 5 to 7 bullets and grounded in the advert.
5. "How this site was built": two sentences on building it with Claude Code and documenting the process on GitHub, with a link to the repo. Position this as evidence of AI workflow fluency.
6. Contact.
Also create a simple root index.html that introduces me in two lines and links to /juicebox/.

TECH
- Plain HTML and CSS, no framework, no build step, no tracking or cookies.
- Mobile first, accessible (semantic headings, alt text, AA contrast), loads fast.
- Clean, professional design with one accent colour. No stock photos.

WORKFLOW
1. Read the inputs, then show me a short plan and the copy for sections 1 and 2. Wait for my approval.
2. Build the pages and run a local preview.
3. Check every claim on the page against the brief and list any that are not supported.
4. Create a .gitignore that excludes advert.md, cv.md and notes.md. Then commit with a clear message. Do not push or publish: I will do that from VS Code. I am a beginner, so explain any step I need to take in plain English.
5. Append a dated entry to docs/build-log.md describing what you did and the prompts used.

EVIDENCE BRIEF
Read @evidence-brief.md in this folder.
```

**Notes:** Replace the company, role, page path and section 4 focus for each application. Update the employer description if my role changes.
