# Meeting Prep Brief

Builds a one-page research brief before a discovery call or sales meeting. Gives you the context to walk in prepared — who you are talking to, what they care about, and what to ask.

## When to Use

Run this skill when you have a meeting booked. You need at least a company name and the person's name. A LinkedIn URL helps but is not required.

## How to Run

Tell Claude: **"Prep me for a meeting with [PERSON NAME] at [COMPANY NAME]"**

Optionally add their LinkedIn URL or any other context you have.

## What It Researches

### 1. The Person
- Current role and how long they have been in it
- Career history — where they came from, what pattern their moves show
- Recent LinkedIn posts or public activity
- Shared connections or mutual context

### 2. The Company
- What they do, explained simply
- Company size, stage, and funding status
- Recent news: launches, fundraises, leadership changes, expansions
- Growth signals: hiring pace, new offices, product launches

### 3. Strategic Context
- Industry trends that affect their business right now
- What their open job postings reveal about priorities
- Likely internal initiatives based on role + company stage

### 4. Call Strategy
- A one-sentence purpose statement for the meeting
- Anchor questions tailored to this specific prospect
- Objections they are likely to raise and how to handle them
- The next step you want to propose at the end of the call

## Starting Point

Before researching from scratch, check if a research brief already exists at `/prospects/research-briefs/[company-name].md`. If it does, use that as your foundation and layer on person-specific and meeting-specific context.

## Output Format

Save the brief as a markdown file:

**Location:** `/prospects/meeting-prep/[company-name]-[person-last-name].md`

**File structure:**

```
# Meeting Prep: [Person Name], [Company Name]
**Date:** [meeting date]
**Prospect:** [Name, Title]
**Meeting Goal:** [one sentence — what you want to learn or accomplish]

---

## Company Snapshot
- [3-5 bullets: what they do, size, stage, recent news, trajectory]

## Person Snapshot
- [3-5 bullets: role, tenure, background, recent activity, anything notable]

## Hypothesis of Pain
- [2-3 bullets: what problems they likely face, with evidence for each]

## Anchor Questions
1. [Specific question tied to their situation — not generic]
2. [Specific question about a trend or challenge in their space]
3. [Question that tests your hypothesis of pain]
4. [Question about their current process or tools]
5. [Question about decision-making or timeline]

## Competitive Notes
- **Current tools:** [what they appear to use based on job postings, tech stack, etc.]
- **Likely evaluating:** [who else they might be comparing you to]

## Desired Outcome
[One sentence: what specific next step you will propose at the end of the call]
```

## Guidelines

- Keep anchor questions specific. "What are your biggest challenges?" is lazy. "You posted about struggling with X — is that still a priority?" is useful.
- The hypothesis of pain should include evidence. Do not guess without reasoning.
- If you cannot find information on something, say so. Do not fabricate details.
- The entire brief should fit on one page when printed. Brevity is the point.
