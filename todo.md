# Roundtable — Pre-launch TODO

## High priority (do before publishing)

- [x] **Resolve the Blog readers panel.** Either replace it with a more generic example panel (e.g. "Product Team") that any user could relate to, or move it into an `Examples/` subfolder with a note explaining it shows what a domain-specific panel looks like. As-is it creates noise next to the five generic default panels.

- [x] **Add an Outputs folder and .gitignore.** Every Panel Feedback and Problem Solving session writes a markdown file into the project root. Create an `Outputs/` subfolder and update AGENTS.md to save sessions there. Add a `.gitignore` to exclude at minimum `.DS_Store` and optionally the Outputs folder if generated content shouldn't be committed.

## Medium priority

- [x] **Fix the Problem Solving prompt.** It currently references "five chosen historical or contemporary figures" internally — a relic from its original design. Replace with generic language so it doesn't produce odd framing when run with non-historical panels like Stakeholder Map or Six Hats.

- [ ] **Standardise persona format across panels.** Time Horizons, Stakeholder Map, and Disciplines panels each have an extra context field near the top (`## Time horizon:`, `## Stakeholder position:`, `## Discipline:`). Historical Figures and Six Hats don't. Decide whether to standardise on including these or document them as optional in the README persona template.

- [ ] **Add example output files.** One example Panel Feedback output and one Problem Solving output would show people what a session actually produces before they commit to trying it. Highest-value item for convincing new users the project is worth using.

## Nice to have

- [ ] Clean up the Expert Persona Generator prompt — it says "return a downloadable markdown file" which is language from Claude's web UI and doesn't fit a Cowork/Code context.
- [ ] Add a note to the README about mixing personas from different panels as a valid workflow.
- [ ] Consider a CONTRIBUTING.md with guidance for people who want to submit new panels.
