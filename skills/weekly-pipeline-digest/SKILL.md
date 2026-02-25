# Weekly Pipeline Digest

## What This Does

Scans everything in your `/prospects/` folder — research briefs, outreach drafts, and meeting prep docs — and builds a single weekly summary. You get a clear picture of what happened, what's working, and what to focus on next week.

## When to Use

- End of week (Friday afternoon is ideal)
- Before a pipeline review or forecast call
- Anytime you want a snapshot of GTM activity without clicking through 20 files

## How to Invoke

Tell Claude Code:

> "Create my weekly pipeline digest"

or

> "Summarize this week's GTM activity"

## What It Reads

| Folder | What It Looks For |
|---|---|
| `/prospects/research-briefs/` | New company research files created or modified this week |
| `/prospects/outreach-drafts/` | Email sequences drafted, their target companies, and status |
| `/prospects/meeting-prep/` | Upcoming meeting briefs with company and contact info |

## Output Format

The digest has six sections:

### 1. Executive Summary
- 3-5 bullets covering: what happened this week, are we on track against goals, and the top risk to flag
- Written for a manager or CRO who has 30 seconds to skim

### 2. New Research Briefs
- Table of companies researched this week
- Includes: company name, ICP tier score (A/B/C), key trigger, and date created
- Sorted by tier (A first)

### 3. Outreach Activity
- Which sequences were drafted or updated
- Target company and contact for each
- Current status: drafted / sent / replied / no response

### 4. Meetings Prep'd
- List of upcoming meetings with prep docs ready
- One-line context per meeting: who, when, and the core hypothesis

### 5. Pipeline Health
- Total prospects in each tier: A, B, C
- Week-over-week change (e.g., "+3 Tier A, -1 Tier B")
- Flags any tier that dropped or has zero new additions

### 6. Action Items
- Top 3 things to prioritize next week
- Derived from gaps in the data: stale prospects, missing follow-ups, meetings without prep

## Output Location

Saved to: `/prospects/weekly-digest-YYYY-MM-DD.md`

Uses the Friday date of the current week.

## Tips

- Run this consistently on the same day so week-over-week comparisons are meaningful
- If a section is empty (e.g., no meetings prepped), the digest will note that explicitly rather than hiding it
- Pair this with the research brief skill to fill gaps the digest surfaces
