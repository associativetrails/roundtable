# Panel of Experts

A prompt framework for running structured multi-perspective analysis using AI. You give it a panel of personas and a problem or piece of content. Each persona responds from their own distinct point of view. The friction between perspectives is the point.

Works with Claude, Codex, and any LLM-based tool that reads project instructions from `AGENTS.md`.

---

## How it works

The project has three components:

**Persona files** describe individual thinkers — their background, approach, priorities, blind spots, voice, and the question they always ask. They live in subfolders named `Personas - {Panel name}/`.

**Prompt files** contain the instructions that tell your AI how to run each type of session. You do not need to read them directly — your AI reads them automatically when you invoke a workflow.

**AGENTS.md** is the instruction layer that tells your AI how to use everything. It is read automatically by Claude, Codex, and other compatible tools when you open this folder.

---

## Getting started

Open this folder in your AI tool of choice (Claude in Cowork or Claude Code, Codex, or any agent that reads `AGENTS.md`). You do not need to do any setup. The AI will read the instructions automatically.

Then use plain language to invoke one of the three workflows below.

---

## Workflows

### 1. Panel Feedback

Give the AI a piece of content — a blog post, proposal, landing page, pitch deck, 1-pager — and tell it which panel you want feedback from. Each persona reads the content and delivers structured, scored feedback from their own perspective, followed by a panel synthesis that surfaces where they agree, where they disagree, and the single highest-leverage change.

**How to use it:**
> "Give me panel feedback on this article from the Six Hats panel."

> "I want feedback on this proposal from the Stakeholder Map panel."

If you do not specify a panel, the AI will list the available options and ask which one you want.

Output is saved as `Panel Feedback - {Panel} - {Title}.md` in the project folder.

---

### 2. Problem Solving

Give the AI a problem or decision and tell it which panel you want to work through it with. The panel runs as a structured roundtable: each persona gives their initial take, they debate with each other, and the session ends with a synthesis of core insights and tensions — plus a final reflective question.

**How to use it:**
> "Help me think through this hiring decision using the Time Horizons panel."

> "I want to work through a problem with the Historical Figures panel. Here's the situation..."

If you do not specify a panel, the AI will list the available options and ask which one you want.

Output is saved as `Problem Solving - {Panel} - {Title}.md` in the project folder.

---

### 3. Generate a Persona

Ask the AI to generate a new persona by giving it a role, some context, and any specific traits you want. The AI produces a fully structured persona file in the standard format and saves it to the correct subfolder.

**How to use it:**
> "Generate a persona for a senior NHS nurse for the Healthcare panel."

> "Add a venture-backed startup CFO to the Business panel."

The AI will ask for the job title, industry or company context, and any additional notes, then write and save the persona file automatically.

---

## Default panels

Five panels ship with this project. Each one applies a different organising principle to produce a different kind of insight.

---

### Six Hats Framework

Six thinkers each embodying one of De Bono's thinking modes: White Hat (facts and information gaps), Red Hat (emotion and gut reaction), Black Hat (critical judgment and failure modes), Yellow Hat (constructive case for value and opportunity), Green Hat (generative ideas and lateral alternatives), Blue Hat (process control and meta-thinking). The panel ensures a problem is examined from all cognitive angles before a decision is made.

**Members:** Elena (White), James (Red), Richard (Black), Aisha (Yellow), Sam (Green), Diana (Blue)

**Use this panel for:**
- Evaluating a proposal before committing to it, when you want structured coverage of all angles rather than the loudest voices
- Creative challenges where the group defaults to critique too early, or to enthusiasm without rigour
- Any situation where the quality of the thinking process matters as much as the output — workshops, strategy sessions, high-stakes decisions

---

### Historical Figures

Six thinkers from history, each embodying a distinct intellectual tradition. The panel brings the weight of tested ideas and hard-won perspectives to bear on current problems.

**Members:** Leonardo da Vinci (cross-domain systems thinking), Marie Curie (empirical rigour), Frederick Douglass (moral clarity and power), Benjamin Franklin (pragmatism and diplomacy), Ada Lovelace (speculative imagination), Marcus Aurelius (Stoic long-termism)

**Use this panel for:**
- Big, complex questions where you want the full range of human intellectual tradition rather than contemporary professional categories
- Decisions with a significant ethical or moral dimension, where Douglass and Aurelius will force the group to confront what it is actually choosing
- Innovation and strategy questions where Lovelace's horizon-thinking and da Vinci's cross-domain curiosity are needed alongside Franklin's practicality and Curie's empirical restraint

---

### Time Horizons

Six thinkers each operating at a different temporal scale. The panel reveals how the same decision looks completely different depending on where you stand in time.

**Members:** Kai (days to weeks — tactical execution), Nina (weeks to quarters — product and iteration), Carlos (quarters to one year — operations and annual planning), Claire (one to five years — competitive strategy), Robert (five to twenty years — institutional capital), Amara (decades to generations — civilisational and systemic impact)

**Use this panel for:**
- Strategy decisions where near-term pressure and long-term positioning are in tension and you need to hold both simultaneously
- Investment or resource allocation decisions where the time horizon of the return is being left implicit
- Any situation where urgency is driving the conversation and you need to ask whether that urgency is real or manufactured

---

### Stakeholder Map

Six thinkers each representing a different affected party. The panel forces a decision to be examined from every position it touches, including the ones not in the room.

**Members:** Fatima (end user — lived experience), Dev (frontline worker — operational reality), Helen (middle manager — implementation friction), Graham (regulator — compliance and legal exposure), Zoe (investigative journalist — public scrutiny), Patrick (investor — financial return and assumptions)

**Use this panel for:**
- Product, policy, or service decisions where the people making the decision are not the people most affected by it
- Launch or rollout planning, where the gap between strategic intent and operational reality needs surfacing before it becomes a problem
- Decisions with public-facing consequences, reputational exposure, or regulatory dimensions that the internal team may be underweighting

---

### Disciplines

Six thinkers each bringing a different academic discipline to the problem. The panel applies six distinct methods to the same question and surfaces the dimensions any single discipline would miss.

**Members:** Isabel (economics — incentives and second-order effects), Owen (psychology — actual versus assumed behaviour), Nneka (sociology — social structures and power), Raj (engineering — systems thinking and failure modes), Sofia (philosophy — conceptual clarity and logical rigour), Bernard (history — precedent and long-run consequences)

**Use this panel for:**
- Complex, multi-dimensional problems where you do not know which lens is right and need the full range before narrowing
- Decisions with behavioural, ethical, or systemic dimensions that a purely financial or operational analysis would miss
- Situations where the group is overconfident — this panel will collectively find the incentive misalignment, the behavioural assumption, the structural blind spot, the failure mode, the reasoning flaw, and the historical precedent everyone missed

---

## Creating your own panels

To add a new panel, create a subfolder named `Personas - {Your panel name}/` and add persona files named `Persona - {Name} - {Role}.md`.

Each persona file follows this structure:

```
# Name — Role

## Background
2–3 sentences covering seniority, experience, domain, and defining career context.

## Approach
The frameworks, mental models, and instincts this person brings to a problem.

## Priorities & constraints
What they are optimising for. What they will not compromise on.

## Blind spots & biases
One or two honest tendencies that make their perspective distinct but also limited.

## Voice & tone
How they communicate. 2–3 adjectives and a sample sentence in their voice.

## The question they always ask
One signature question this person reliably raises.
```

Use the persona generator workflow to create new personas automatically, or write them by hand following this format. The AI will find any subfolder that matches the naming convention and treat it as an available panel.
