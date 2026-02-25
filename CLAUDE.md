# Claude Instructions for The GTM Engineer Toolkit

## Who I Am

I'm a non-technical [YOUR ROLE] at [YOUR COMPANY].
I work in Go-To-Market — sales, marketing, partnerships, or some mix of all three.
I don't write code. I understand pipeline, personas, and positioning — not Python.

---

## How to Talk to Me

- **Plain English only.** If you must use a technical term, explain it immediately.
- **Use analogies.** Relate technical concepts to GTM concepts I already know.
- **Always explain what you're doing and why** before you do it.
- **Connect every step to a business outcome.** "This pulls firmographic data so you can prioritize accounts that match your ICP" — not "this parses the JSON response."
- **Suggest the simplest path first.** Don't over-engineer. If there's an easier way, say so.

---

## Project Context

This is a GTM workflow toolkit. It contains skills (reusable prompt files) for:
- **Prospect Research** — Build research briefs on target accounts
- **ICP Scoring** — Score leads against your Ideal Customer Profile
- **Outreach Writing** — Draft personalized cold emails and sequences
- **Meeting Prep** — Generate pre-call briefs with talking points
- **Pipeline Reporting** — Summarize deal status and flag risks

When a task matches one of these workflows, **use the relevant skill file:**
- `skills/icp-scorer/SKILL.md`
- `skills/prospect-researcher/SKILL.md`
- `skills/cold-outreach-writer/SKILL.md`
- `skills/meeting-prep-brief/SKILL.md`
- `skills/weekly-pipeline-digest/SKILL.md`

---

## Key Rules

1. **Explain as you go.** Tell me what you're about to do, then do it.
2. **Highlight business impact.** Every output should answer "so what?" for a GTM person.
3. **Use bullet points, headers, and short paragraphs.** I skim before I read.
4. **When I get stuck,** ask one clarifying question, reframe in business terms, then offer 2-3 simple options.
5. **Give me copy-paste ready outputs.** If I need to send an email, give me the email — not instructions on how to write one.

---

## Before You Run Anything

**Customize the ICP Scorer first.** The ICP scoring skill ships with placeholder criteria. Before running any research or scoring workflow, update `skills/icp-scorer/SKILL.md` with your actual ICP — company size, industry, tech stack, whatever matters to your business. There is a fill-in-the-blank template at `templates/starter-icp-template.md` to make this easier. Everything else builds on this.

---

## Security Note

If you install skills or extensions from outside this repo, **review them before running.** Skills are just text files with instructions — read them first to make sure they do what you expect. When in doubt, ask Claude to explain what a skill does before you use it.
