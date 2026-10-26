# Build log

## 26 October 2026: first build of the Juicebox application site

**Tool:** Claude Code (Opus 5.5) in VS Code

### What was done

1. **Read the inputs.** The Juicebox job advert, my CV and an evidence brief mapping each requirement in the advert to my evidence and results. No PDF CV was available, so the CV download link points to `assets/cv.pdf` as a placeholder.
2. **Planned and drafted copy for approval.** Claude proposed a file structure and drafted the hero and the "Your advert, my evidence" table, then listed nine questions where the brief and CV disagreed or a fact was missing, instead of guessing.
3. **Resolved the questions.** My answers corrected or clarified several facts (see "Prompts used" below).
4. **Built the pages.** Plain HTML and one CSS file, no JavaScript, web fonts, cookies or tracking:
   - `index.html`: two-line introduction linking to `/juicebox/`
   - `juicebox/index.html`: hero, evidence table, three case studies, 90-day plan, how the site was built, contact
   - `assets/styles.css`: mobile first, one teal accent, colours chosen for WCAG AA contrast; the evidence table turns into stacked cards on phones
5. **Previewed locally** at `http://127.0.0.1:8000/`. Python was not available in the session, so a small PowerShell web server was used instead.
6. **Checked the copy.** Confirmed no em or en dashes, case studies at 77, 101 and 66 words (limit 120), and checked every claim against the evidence brief. Two lines were softened as a result: "searches and outreach" became "searches" (the advert does not mention outreach), and "each prompt and decision is documented" became "the prompts and steps are documented".
7. **Set up git and GitHub.** Created `.gitignore` (excludes `advert.md`, `cv.md`, `notes.md`), initialised the repository, made the first commit, and created an empty public repository at https://github.com/blkren/portfolio connected as `origin`. Nothing was pushed. `evidence-brief.md` was left out of the commit because it still contains figures I later corrected.

### Prompts used

**Main prompt (summary).** Build a portfolio site for a Customer Success Manager application at Juicebox whose single job is to show, quickly and with evidence, why I match the advert. Rules: UK English, no em dashes, no hype words, frame achievements around customer and business outcomes, never invent or round up a number, no client names or confidential detail from my current employer (describe it as "a UK professional services compliance business serving 3,000 schools and trusts"). Specified the page structure, plain HTML and CSS, accessibility, and a workflow: plan and approve copy, build and preview, check claims, commit without pushing, write this log.

**Clarifying answers I gave:**

- Name and contact details to show on the site, and a request to create the GitHub repository.
- The two central government departments were two of my top five accounts (two contracts, not four).
- 82% of cancellations have been processed through my new process over the last ten months, before it becomes the required process in new contract terms.
- Databricks Genie One and Agent Bricks were added to the roadmap, not the Copilot Studio digital workforce.
- My NRR target at Be Applied was 110%, and I averaged 122% across the year.
- Elev8 Performance UK ran for six years, not seven.
- Use "within eight weeks" for the at-risk client turnaround, to match my CV.
- I am available to work on-site in London.

### Still to do

- Add `cv.pdf` to `assets/`.
- Push to GitHub and publish the site.
