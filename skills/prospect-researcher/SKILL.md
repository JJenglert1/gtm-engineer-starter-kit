# Prospect Researcher

Build a concise, actionable research brief on any company or prospect in about 2-3 minutes. Give it a company name, URL, or a list of prospects and get back structured briefs you can hand straight to a seller.

## When to Use

Invoke this skill when you have a company name, website URL, or a list of prospects and you need to understand who they are, what they care about, and how to open a conversation. Run it before writing outreach, before a first call, or when qualifying a new lead.

## How It Works

Use web search and, when available, the agent browser skill to pull information from public sources. Do not spend 20 minutes going deep. Aim for the most useful 80% of insight in 2-3 minutes per company. Move fast, flag gaps, and move on.

## Research Framework

Gather information from these five categories in order of priority:

### 1. Company Fundamentals
- Company website: about page, product pages, pricing page
- Recent blog posts or press releases (last 90 days)
- Crunchbase or PitchBook profile for funding and size
- One-sentence summary of what they sell and to whom

### 2. People Intelligence
- Prospect's current title and how long they have been in the role
- Career history: where they came from, how long at prior companies
- Recent LinkedIn posts or public activity (topics they care about)
- Any podcast appearances, conference talks, or published writing

### 3. Trigger Events
- Funding rounds in the last 6 months
- Executive hires or departures
- Job postings that signal new initiatives (look for titles and tools mentioned)
- Product launches, partnerships, or expansion announcements
- Earnings calls or analyst mentions (for public companies)

### 4. Tech Stack Clues
- Check their website source and job postings for tools mentioned
- Look for case studies or integration pages on vendor sites
- Note any tools relevant to [YOUR PRODUCT CATEGORY]

### 5. Competitive Context
- What competitors or alternatives do they currently use
- G2 or Capterra reviews they have left or received
- Any public complaints or praise about current solutions

## Output Format

Save each brief as: `prospects/research-briefs/[company-name].md`

Structure the output exactly like this:

```
# Research Brief: [Company Name]
Date: [today's date]
Source: [primary URLs used]

## Company Snapshot
[2-3 sentences: what they do, who they sell to, approximate size and stage.]

## Recent Trigger
[The single most relevant event in the last 90 days and one sentence on why it matters for your outreach.]

## Likely Pain
[Your hypothesis on what problem they face that your product solves. Base this on their stage, recent hires, tech stack, or competitive situation. Be specific, not generic.]

## Tech Stack
[List the key tools you found, especially ones relevant to your product. Note where you found each clue (job posting, website, integration page).]

## Stakeholder Notes
[Prospect's name, title, tenure in role, and one relevant observation from their public activity. If multiple stakeholders, list the top 2-3.]

## Proposed Hook
[One sentence: the specific angle you would use to open a conversation with this person at this company right now.]
```

## Handling Lists

When given a list of prospects, process them one at a time. Save each brief as its own file. After finishing the list, produce a summary table:

```
| Company | Trigger | Proposed Hook | Brief Link |
|---|---|---|---|
| Acme Corp | Series B funding | ... | [link to file] |
```

## Tips for Better Results

- **Start with the trigger.** The most useful part of any brief is the recent event that gives you a reason to reach out now. Find that first.
- **Be specific about pain.** "They probably need better analytics" is useless. "They just hired 3 data engineers and are posting for a head of BI, which suggests they are outgrowing their current stack" is useful.
- **Skip what you cannot find.** If a section has no available information, write "Not found" and move on. Do not pad with filler.
- **Customize the tech stack section.** Replace [YOUR PRODUCT CATEGORY] above with your actual category so the skill knows which tools to flag as relevant.

## Before First Use

- [ ] Replace [YOUR PRODUCT CATEGORY] with your actual product category
- [ ] Confirm you have web search or agent browser available for research
