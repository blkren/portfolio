# Documentation setup

**Purpose:** Standing rules, a documentation plan and a templated folder structure that show how a repo was built, not just the result.

**Inputs:** An existing repo, a folder outline, and the templates in `docs/documentation-plan.md`.

**Prompt:**

```
Create a documentation plan for this repository and set up the files to support it. The repo is a public portfolio used in job applications. Its audience is hiring managers and CS leaders who will spend two minutes on it. It should show how I use AI tools to build things, not just the finished site.

1. Create CLAUDE.md with standing rules for every session in this repo: UK English, no em dashes, confident but grounded tone; never invent metrics, ask me if a fact is missing; no client names, internal financials or confidential employer detail; at the end of every session, append an entry to docs/build-log.md; save any reusable prompt to prompts/ using the prompt template.
2. Write docs/documentation-plan.md covering what gets documented, when, a commit message convention (type: short description; types: build, content, docs, fix) and a one-line rule for what never goes in the repo.
3. Create the folder structure from the outline I give you next, using the templates provided. Populate the files from what we have already built and from cv.md. Where you do not have a fact, leave a [fill in] marker and list every marker for me at the end. Fill the case studies from the evidence brief, keeping each under 250 words.
4. Show me the plan and file tree before committing. Then commit. Do not push.

Keep every file short. If a section would be empty, leave it out rather than writing filler.
```

**Notes:** Paste the folder outline and templates after the prompt. Change the audience line if the repo is for something other than job applications.
