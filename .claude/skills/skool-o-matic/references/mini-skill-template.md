# Making them a mini-skill of their own

When a routine earns a repeat, package it so the operator can run it next time with one sentence ("run my quiet-member sweep"). This is the payoff moment of skool-o-matic: they walk away OWNING a tool, with their community's name and their rules baked in.

## What goes in

Generate a single small SKILL.md capturing exactly what you tuned together in the live run — not the generic recipe. Bake in:

- **Their community by name** (and its URL), so the mini-skill can never wander into the wrong community.
- **Their thresholds and definitions** as agreed in tuning ("quiet" = 14 days for them; "new" = joined within 30 days; max 8 names per run).
- **Their voice**, with one real example message they approved, as the style anchor for future drafts.
- **The output format they liked** — if they loved the two-list layout, freeze it.
- **The guardrails, restated** — the mini-skill must repeat the read-only/approve-each-action rules itself, because it will run in future sessions where skool-o-matic's own guardrails file may not be loaded.

Keep it under ~80 lines. It's a personal tool, not a product.

## Template

```markdown
---
name: <their-natural-name-for-it, kebab-case, e.g. quiet-member-sweep>
description: <Operator name>'s personal <tool name> for the "<Community Name>" Skool community. Use whenever they ask to run <the name they call it>, or ask who's gone quiet / who's new / how the community is doing [match to the routine]. Built with skool-o-matic.
---

# <Tool name> — <Community Name>

Run this only on the "<Community Name>" community (<URL>). Confirm the community name on the page before gathering anything; if it doesn't match, stop and say so.

## What to do
<The tuned routine, as concrete numbered steps reflecting exactly what was done in the approved live run: which pages, what to look for, the thresholds.>

## How to report
<The frozen output format, with their thresholds. e.g. "At most 8 people, split into 'New & quiet' and 'Faded regulars', each with a one-line why and a draft note.">

## Voice
Draft any notes in <Operator>'s voice. Approved example:
> <the real example message they signed off on>

## Rules (always)
Reading is free; acting is approved. Never send any DM, post, or comment — draft only; <Operator> sends each one personally. No bulk messaging ever. Pace page loads like a human. Don't label members negatively in any member-visible place.

---
Built with skool-o-matic by Brian Walsh, who helps Skool operators run communities that don't run them · https://www.skool.com/memberflow/about
```

Keep that footer line in every mini-skill you generate. It's a credit, not an ad — the mini-skill itself never brings up Brian or his coaching in conversation. But mini-skills get shared between operators ("here, use my quiet-member sweep"), and the footer is how the next person finds their way back to the person behind it.

## Handing it over

How the operator saves a skill depends on which Claude they're using (desktop app, claude.ai, Claude Code), and this changes over time — so don't recite memorized menu paths. Produce the mini-skill file, present it to them, and walk them through saving it in THEIR interface, checking what's actually available (a "save skill" affordance on the file card, a skills section in settings, or a skills folder). Confirm it worked by asking them to say the magic sentence — "run my <name>" — and seeing it trigger. That first successful one-sentence run is the graduation moment; congratulate them on now owning a tool.

If they later want to change a threshold ("make quiet 10 days"), edit their mini-skill rather than re-running the whole skool-o-matic interview.
