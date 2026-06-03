# Roundtable Design System

This document describes the visual design language for Roundtable session outputs. It is the authoritative reference for generating both HTML (see `template.html`) and Word documents. All outputs should follow these conventions regardless of format.

---

## Principles

- Typography does the heavy lifting. Spacing and weight create hierarchy, not colour or decoration.
- White space is generous. Content is not crowded.
- Each module has a clear, distinct job. Do not blend module types.
- Labels are always small caps / uppercase. Content text is always sentence case.

---

## Typography

**Typeface:** Helvetica Neue (fallback: Helvetica, Arial, sans-serif). In Word, use Calibri or Arial as the closest available equivalent.

**Body text:** 15px / 1.65 line-height / colour #222. In Word: 11pt, 1.5 line spacing.

**All labels and metadata** (session type line, verdict labels, action labels, footer) are uppercase, tracked out, small and subdued. Colour #888. In Word: use ALL CAPS with character spacing expanded ~2pt, colour mid-grey.

---

## Colour palette

| Role | Hex | Usage |
|---|---|---|
| Near-black | #111 | Titles, headings, pull quote text, persona names |
| Dark body | #222 | Body prose |
| Mid body | #333 | Stat labels, verdict body text |
| Grey label | #888 | All metadata labels, persona roles, citations |
| Light grey | #aaa | Stat source attribution, footer text |
| Rule grey | #ddd / #e8e8e8 | Horizontal rules, borders |
| Background | #f5f5f5 | Action block background |
| Hero band | #777 | Hero background (mid-grey) |
| Hero text | #fff | All text inside the hero band |
| Verdict — good | #d4a017 (border) / #a07a00 (label) | "What good looks like" left border and label |
| Verdict — bad | #d63a1e (border) / #b03010 (label) | "What bad looks like" left border and label |
| Verdict — neutral | #888 (border) / #666 (label) | Neutral verdict or "needs investigation" |

---

## Modules

### Session type line
Small caps metadata line sitting above the page title. Format: `Session Type · Panel Name · Date`. Colour #888, uppercase, tracked.

In Word: style as a custom character style — Calibri 9pt, ALL CAPS, character spacing +2pt, colour mid-grey. No paragraph border.

---

### Page title
The main title of the session. Large, bold, tight letter-spacing. Colour #111.

In Word: Heading 1 style. Arial Bold, 26pt, colour black, space before 48pt, space after 24pt.

---

### Hero band
A full-width grey band (#777) with white text. Contains two elements:
- **Hero subtitle:** bold, 22px, the key framing statement or question
- **Hero body:** smaller, slightly transparent, one or two sentences of context

In Word: simulate with a shaded paragraph block — grey fill (#777777), white text. Subtitle in Arial Bold 16pt, body in Arial 11pt. Add 24pt padding top and bottom via paragraph spacing.

---

### Section heading (H2)
Bold, 22px, colour #111, generous space above. Marks major structural divisions (e.g. "Diagnostic pass", "Root cause map", "Recommended workflow").

In Word: Heading 2 style. Arial Bold, 16pt, colour black, space before 36pt, space after 10pt.

---

### Sub-heading (H3)
Bold, 16px, colour #111. Used for secondary structure within a section.

In Word: Heading 3 style. Arial Bold, 12pt, colour black, space before 20pt, space after 6pt.

---

### Persona header
Marks the start of each persona's contribution. Two lines:
- **Name:** bold, 18px, colour #111
- **Role:** small caps, 12px, colour #888, uppercase

Preceded by a 2px solid black top border with generous space above.

In Word: Name in Arial Bold 13pt, colour black. Role in Arial 9pt, ALL CAPS, colour mid-grey. Add a paragraph border (top rule, 1.5pt, black) to the name paragraph with 24pt space before.

---

### Body prose
Standard paragraphs. 15px, line-height 1.65, colour #222. No indentation. Space between paragraphs.

In Word: Normal style. Calibri 11pt, 1.5 line spacing, space after 8pt, no indent.

---

### Pull quote
A significant statement lifted from the panel discussion. Left border (3px solid #111), indented. Text is larger and bolder than body prose. Attribution sits below in small caps grey.

In Word: Use the built-in Quote or Intense Quote style, or create a custom style — left border 2.25pt black, text Arial Semi-Bold 14pt colour black, attribution Arial 9pt ALL CAPS colour mid-grey. Indent left 18pt.

---

### Statistic callout
A large centred number with a short descriptor and an optional source attribution. Used sparingly — one per session at most. The number is very large (72px / 800 weight). The descriptor is 14px centred. The source is tiny, uppercase, very light grey.

In Word: Number in Arial Black or Arial Bold 48pt, centred, colour black. Descriptor in Calibri 10pt, centred, colour #333. Source in Calibri 8pt, ALL CAPS, centred, colour light grey. Surround with generous paragraph spacing (24pt before and after the block).

---

### Verdict block (good / bad / neutral)
A left-bordered block used for "What good looks like", "What bad looks like", or similar comparative statements. Three variants:

- **Good:** amber border (#d4a017), amber label (#a07a00)
- **Bad:** red border (#d63a1e), red label (#b03010)
- **Neutral:** grey border (#888), grey label (#666)

Each block has a small uppercase label above the body text.

In Word: Left paragraph border, 2.25pt, coloured to match variant. Label in 8pt ALL CAPS with matching colour. Body in Calibri 10pt colour #333. Space before block 12pt, space after 12pt. Indent left 14pt.

---

### Action block
A light grey background block (#f5f5f5) with an uppercase label and one or more body paragraphs. Used for structured findings: "Confirmed causes", "Suspected cause", "Needs investigation", etc.

In Word: Shaded paragraph, light grey fill (#F5F5F5), no border. Label in Calibri 8pt ALL CAPS colour mid-grey. Body in Calibri 10pt colour #222. Padding via paragraph spacing — 12pt before first paragraph, 12pt after last. Indent left and right 14pt.

---

### Numbered step list
An ordered list with bold circled numbers. Used for the recommended workflow sequence. Steps have bold lead text followed by explanation.

In Word: Standard numbered list. Numbers in Arial Bold, list text in Calibri 11pt. Bold the first clause of each item (the action). Space after each item 6pt.

---

### Open questions
A closing section separated by a top rule. A small uppercase label ("Open questions") followed by individual question items, each separated by a light rule.

In Word: Section label in Calibri 8pt ALL CAPS colour mid-grey, paragraph border top 0.75pt grey, space before 36pt. Each question in Arial Semi-Bold or Bold 12pt colour black, paragraph border bottom 0.75pt light grey, space after 8pt.

---

### Horizontal rule / divider
A light 1px grey rule used to separate major sections within the body. Colour #e8e8e8.

In Word: Paragraph bottom border, 0.75pt, colour light grey (#E8E8E8), space before and after 24pt.

---

### Footer
Small, uppercase, very light grey. Contains session metadata: `Roundtable · Session Type · Panel · Date`.

In Word: Calibri 8pt, ALL CAPS, colour light grey, space before 36pt, paragraph border top 0.75pt light grey.

---

## Optional persona fields

Some panels include an extra context field immediately after the persona name, before `## Background`. This field is optional — it exists to surface the organising principle of the panel at a glance, and is most useful in panels where each persona represents a distinct category (a time horizon, a stakeholder position, a discipline).

The field takes the form `## {Category}: {value}`, for example:

- `## Time horizon: days to weeks`
- `## Stakeholder position: the person the decision is ultimately for`
- `## Discipline: economics`

Do not add this field to personas that don't already have it. Do not require it when generating new personas unless the panel's organising logic makes it genuinely meaningful. If you are generating a persona for a panel where the other personas include this field, add a matching one for consistency.

---

## Document structure

Every session output follows this order:

1. Session type line
2. Page title
3. Hero band (subtitle + context)
4. Body intro (one or two paragraphs orienting the reader)
5. Session content (sections, personas, findings — varies by session type)
6. Open questions
7. Footer

Do not skip the hero band. Do not skip the open questions. These bookend the session and are part of every output regardless of format.
