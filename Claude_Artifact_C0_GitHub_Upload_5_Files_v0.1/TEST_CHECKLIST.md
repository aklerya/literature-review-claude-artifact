# Reproducibility test checklist (C0 — GitHub → Personal Artifact)

**Gate 1 — Source fidelity**
- [ ] New user downloads the HTML source from the expected repository without signing into the repository owner’s GitHub account.
- [ ] New user can attach it in Claude and request a new interactive Artifact.
- [ ] Generated UI contains the research question field, functional button and 3-result display.

**Gate 2 — Runtime + actual AI**
- [ ] Artifact requests Use Claude permission as expected.
- [ ] English question returns exactly 3 topic-specific English subquestions.
- [ ] Completely different Hebrew question returns exactly 3 Hebrew subquestions with RTL layout.
- [ ] Blank input produces an error, not an invented response.
- [ ] When permission is denied or a limit is hit, UI displays a failure rather than a fake success.
- [ ] No personal API key or additional paid service required.

**Gate 3 — Independent distribution**
- [ ] An independent Claude account repeats Gate 1–2.
- [ ] Record number of steps, time and any subscription/permission requirements.
- [ ] Save screenshot and describe outcome; label C0 distribution passed only if this completes.

**Out of scope:** real article search, citations, reliable evidence extraction, long-term persistence, PDF/DOCX export, full MVP security audit. Directly opening this HTML outside Claude is not a valid AI execution test.
