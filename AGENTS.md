## Contents

This project contains:
* Two subfolders containing panels of personas:
	* `/_examplepanels` contains panels that are included in the Roundtable repository
	* `/_custompanels` is initially empty - when the user builds their own panels, store them in this folder
* The persona subfolders are named `Panel - {Group name}/`, each containing persona files named `Persona - {Name} - {Role}.md`
* An output folder `/_output` which is where the panel outputs are saved
- `Prompt - Expert Persona Generator.md` — instructions for generating a new persona
- `Prompt - Panel Feedback.md` — instructions for running a panel feedback session
- `Prompt - Problem Solving.md` — instructions for running a problem-solving roundtable

---
## Lists of panels

When you need to return a list of the available panels, go through both  `/_examplepanels` and `/_custompanels` and return the panel titles, indicating which folder they are in.

---
## Start a new panel

When the user wants to start a new panel, create a subfolder in the `/_custompanels` folder with the name `Panel - {Title}`. Ask the user for the title.

---
## Generate a persona

When the user asks to generate a persona, read `Prompt - Expert Persona Generator.md` and follow its instructions exactly. Save the output as `Persona - {Name} - {Role}.md` in the subfolder the user specifies, or ask which subfolder to use if they have not said.

---
## Panel Feedback - for direct feedback on a document or text
When the user asks for panel feedback, they will provide a document to assess and a reference to a panel (e.g. "Six Hats" or "Stakeholder Map").

If no panel is specified, list the available options by reading the subfolder names and ask the user which one they want.

Once a panel is identified, read all persona files in the matching subfolder (`Personas - {Group name}/Persona - {Name} - {Role}.md`). Inject those personas into the prompt found in `Prompt - Panel Feedback.md` and run the session.

Save the output as `Panel Feedback - {Group} - {Title of document}.md` in the `/_output folder.

---

## Problem Solving - when working through a problem or issue
When the user asks for help problem solving, they will provide a problem or decision to work through and a reference to a panel.

If no panel is specified, list the available options by reading the subfolder names and ask the user which one they want.

Once a panel is identified, read all persona files in the matching subfolder (`Personas - {Group name}/Persona - {Name} - {Role}.md`). Inject those personas into the prompt found in `Prompt - Problem Solving.md` and run the session.

Save the output as `Problem Solving - {Group} - {Title of document}.md` in the `/_output` folder.

---

## Decision making - for help in making a decision
When the user asks for help making a decision, ask them to provide decision to work through and a reference to a panel.

If no panel is specified, list the available options by reading the subfolder names and ask the user which one they want.

Once a panel is identified, read all persona files in the matching subfolder (`Personas - {Group name}/Persona - {Name} - {Role}.md`). Inject those personas into the prompt found in `Prompt - Board of Directors.md` and run the session.

Save the output as `Desicion making - {Group} - {Title of document}.md` in the `/_output` folder.


---

## Panel selection guidance

If the user has not specified a panel and needs a recommendation, use the following to guide the suggestion:

- **Six Hats Framework** — best when the user wants structured cognitive coverage of all angles before making a decision, or when a creative or strategic session needs process discipline
- **Historical Figures** — best for big, complex questions with ethical dimensions, or when the user wants the full breadth of human intellectual tradition rather than contemporary professional categories
- **Time Horizons** — best when near-term pressure and long-term positioning are in tension, or when urgency is driving the conversation and needs to be examined
- **Stakeholder Map** — best when the decision affects people not in the room, or when the gap between strategic intent and operational reality needs surfacing
- **Disciplines** — best for multi-dimensional problems where no single lens is obviously right, or when the group may be overconfident and needs the full range of methods applied simultaneously
