# 002: Evidence table becomes stacked cards on phones

**Date:** 2026-10-26

**Options considered:** A table that scrolls sideways on phones; a table that turns into one card per requirement

**Chosen:** Stacked cards

**Why:** On a phone, sideways scrolling hides the result column, which is the point of the table. Cards keep each requirement, evidence and result together.

**Trade-off accepted:** Extra CSS and ARIA roles are needed to keep the table accessible to screen readers.
