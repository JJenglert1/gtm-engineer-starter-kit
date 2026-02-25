# Cold Outreach Writer

Generates a personalized 3-email outreach sequence for a prospect. Each email is short, human, and built around a specific signal — not a generic pitch.

## When to Use

Run this skill after a research brief already exists in `/prospects/research-briefs/`. You need that context to write emails worth reading.

## How to Run

Tell Claude: **"Write a cold outreach sequence for [COMPANY NAME]"**

Claude will pull the research brief, identify the strongest signal, and draft all three emails.

## Core Principles

- **Signal-based personalization.** Every first line must reference something specific — a job posting, a funding round, a LinkedIn post, a product launch. If you cannot point to the source, the personalization is not real.
- **Short emails.** First touch: under 80 words. Follow-ups: 50-125 words. Count them.
- **One CTA per email.** Never ask two things. The ask must be low-friction: a 15-minute call, a yes/no reply, watching a 2-minute video. Never "let me know a good time" without proposing one.
- **Write like a person.** Target a 5th-6th grade reading level. Short sentences. No jargon. Read it out loud — if it sounds like marketing copy, rewrite it.

## The 3-Email Sequence

### Email 1 — First Touch (Send Day 1)

Structure: Signal observation → connect it to a problem they likely have → one simple CTA.

Subject line: 3-7 words. Curiosity or benefit driven. Lowercase is fine.

The entire email should be under 80 words. Get in, make your point, get out.

### Email 2 — Value-Add Follow-Up (Send Day 3-5)

Structure: One-line callback to the previous email → share something genuinely useful (a relevant case study, a data point, a short insight) → repeat or rephrase the CTA.

Do not apologize for emailing again. Do not say "just following up."

### Email 3 — Breakup (Send Day 14-17)

Structure: Acknowledge the silence without guilt-tripping → offer one final piece of value → give them explicit permission to say no → warm close.

The goal is to leave the door open, not to pressure.

## Anti-Patterns — Never Do These

- Open with "I hope this email finds you well"
- Open with "My name is X and I work at Y"
- Say "Just following up" or "Bumping this to the top of your inbox"
- Dump features or pitch your product in Email 1
- Put multiple CTAs in one email
- Use spam words: "free", "guaranteed", "act now", "limited time", "exclusive offer"
- Use the "No X needed, just Y" parallel structure — it is an obvious AI writing tell
- Write subject lines longer than 7 words
- Use exclamation points in subject lines

## Subject Line Rules

- 3-7 words only
- Lowercase is fine and often outperforms title case
- Spark curiosity or state a clear benefit
- Never mislead — the subject must connect to the email body
- Examples of good patterns: "quick question about [their initiative]", "[competitor] vs your approach", "saw your [specific thing]"

## Output Format

Save all three emails as a single markdown file:

**Location:** `/prospects/outreach-drafts/[company-name].md`

**File structure:**
```
# Outreach Sequence: [Company Name]
**Prospect:** [Name, Title]
**Signal Used:** [what triggered this outreach]
**Created:** [date]

---

## Email 1 — First Touch (Day 1)
**Subject:** [subject line]

[body]

---

## Email 2 — Value-Add Follow-Up (Day 3-5)
**Subject:** [subject line]

[body]

---

## Email 3 — Breakup (Day 14-17)
**Subject:** [subject line]

[body]
```

## Placeholders

Replace these with your real info before sending:
- `[YOUR COMPANY NAME]` — your company
- `[YOUR VALUE PROP IN ONE SENTENCE]` — what you do, stated simply

## Quality Check

Before finishing, verify each email against this list:
1. Is the word count within range?
2. Is there exactly one CTA?
3. Does the personalization reference a real, specific signal?
4. Would you actually read this if it landed in your inbox?
