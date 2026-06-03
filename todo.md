# Roundtable — Pre-launch TODO

---

## Must do before publishing

- [x] **Decide what to do with the Blog Readers panel.** It lives in `/_custompanels` and is currently gitignored, so it won't ship — but the panel itself is domain-specific to Associative Trails. Either move a cleaned-up version to `/_examplepanels` as a demonstration of what a custom panel looks like, or leave it excluded. Either way, make the call consciously.

- [x] **Add example output files.** The README promises users can see what a session produces, but there are no examples in the repo. Generate one clean example for each of the three session types (Panel Feedback, Problem Solving, Decision Making) using an example panel, and save them somewhere visible — either in a top-level `/_examples` folder or linked from the README. This is the highest-value thing for convincing new users the project is worth using.

- [x] **Check the `_output` folder before pushing.** It contains a real session (`Boardroom Simulation - Six Hats - Associative Trails Pivot.md`) with what looks like internal Associative Trails content. The folder is gitignored so it won't push, but confirm the gitignore is working correctly (`git status`) before publishing.

- [x] **Standardise persona format across panels.** Time Horizons, Stakeholder Map, and Disciplines panels each have an extra context field near the top (`## Time horizon:`, `## Stakeholder position:`, `## Discipline:`). Historical Figures and Six Hats don't. Decide whether to standardise on including these or document them as optional in `/_assets/DESIGN.md` and the README persona template.

- [x] **Test all three workflows end to end.** Run one Panel Feedback, one Problem Solving, and one Decision Making session from a cold start in a fresh Claude conversation. Verify the AI reads AGENTS.md correctly, asks the right questions, picks up the right prompt file, runs the session, asks for output format, and saves to `/_output` with the right filename. Fix anything that breaks.

- [x] **Test all three output formats.** For at least one session, generate the output in each of the three formats (Markdown, Word, HTML) and check they're usable. In particular, confirm the HTML output matches `/_assets/template.html` and the Word output follows `/_assets/DESIGN.md`.

---

## Should do before a big announcement

- [ ] **Write a short `CONTRIBUTING.md`.** If you're publishing this publicly and want people to submit panels, they need to know how. Cover: the persona file format, the naming convention, where custom panels live, and how to submit a PR.

- [x] **Add a licence file.** Decide on a licence (MIT is the obvious choice for an open framework) and add a `LICENSE` file. Without it, the default is "all rights reserved" which is probably not the intent.

- [x] **Clean up the Expert Persona Generator prompt.** It currently says "return a downloadable markdown file" — language from Claude's web UI that doesn't fit a Cowork or Claude Code context. Update it to say "save the file to the specified subfolder."

- [x] **Consider whether `CLAUDE.md` should be in the repo.** It currently just says `@AGENTS.md`. Fine to include, but make sure it doesn't contain anything session-specific or AT-internal before it goes public.

- [x] **Add a social preview image.** GitHub shows the `og:image` on link previews. A simple image with the Roundtable name and a one-line description will make the repo look intentional when people share it.

---

## Nice to have

- [ ] Add a note to the README about mixing personas from different panels as a valid workflow.
- [ ] Consider whether `/_assets/template.html` should be described in the README so users know it exists and what it's for.
- [ ] Add a `CHANGELOG.md` or release notes if you plan to version the framework over time.
