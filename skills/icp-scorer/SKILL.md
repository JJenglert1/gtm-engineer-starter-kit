# ICP Scorer

Score any prospect against your Ideal Customer Profile to decide if they are worth pursuing right now, worth nurturing, or not a fit. Hand it a company name or URL and get back a structured scorecard.

## When to Use

Invoke this skill when you need to evaluate whether a prospect is a good fit before spending time on outreach. Run it on new inbound leads, prospect lists, or any company you are considering adding to your pipeline.

## Scoring Framework (100 points total)

### 1. Firmographic Fit (40 points)

| Signal | Points | Your Target |
|---|---|---|
| Industry match | 0-10 | [YOUR TARGET INDUSTRIES, e.g. B2B SaaS, fintech, healthtech] |
| Company size (headcount) | 0-10 | [YOUR IDEAL HEADCOUNT RANGE, e.g. 50-500 employees] |
| Revenue range | 0-10 | [YOUR IDEAL REVENUE RANGE, e.g. $5M-$100M ARR] |
| Geography | 0-5 | [YOUR TARGET GEOS, e.g. US, Canada, UK] |
| Business model alignment | 0-5 | [YOUR IDEAL MODEL, e.g. subscription, usage-based] |

### 2. Technographic Fit (20 points)

| Signal | Points | Your Target |
|---|---|---|
| Uses compatible tech stack | 0-10 | [TECH YOUR PRODUCT INTEGRATES WITH, e.g. Salesforce, HubSpot] |
| Uses complementary tools | 0-10 | [TOOLS THAT SIGNAL READINESS, e.g. Outreach, Gong, Snowflake] |

### 3. Intent and Behavioral Signals (25 points)

| Signal | Points | How to Check |
|---|---|---|
| Visited your website or pricing page | 0-8 | Check your analytics or intent data platform |
| Downloaded content or attended webinar | 0-7 | Check your CRM or marketing automation |
| Researching your product category | 0-5 | Search for G2, Capterra, or analyst report activity |
| Reading competitor reviews | 0-5 | Look for G2 compare pages, Reddit threads |

### 4. Trigger Events (15 points)

| Signal | Points | How to Check |
|---|---|---|
| Recent funding round | 0-5 | News search, Crunchbase |
| New executive hire in relevant role | 0-4 | LinkedIn, press releases |
| Headcount growth in key departments | 0-3 | LinkedIn jobs page, hiring signals |
| Product launch or expansion | 0-3 | Blog, press releases, Product Hunt |

## Score Thresholds

- **Tier A (85-100):** Immediate outreach. Strong fit across multiple categories. Prioritize this week.
- **Tier B (60-84):** Nurture and monitor. Good fit but missing intent or trigger signals. Add to sequences and revisit monthly.
- **Tier C (Below 60):** Deprioritize. Weak fit or no active signals. Do not spend outbound effort here.

## Output Format

Save the scorecard as a markdown file at: `prospects/research-briefs/[company-name]-icp-score.md`

Structure the output exactly like this:

```
# ICP Scorecard: [Company Name]
Date: [today's date]

## Scores
| Category | Score | Max | Notes |
|---|---|---|---|
| Firmographic Fit | X | 40 | [brief rationale] |
| Technographic Fit | X | 20 | [brief rationale] |
| Intent/Behavioral | X | 25 | [brief rationale] |
| Trigger Events | X | 15 | [brief rationale] |
| **Total** | **X** | **100** | |

## Tier: [A / B / C]

## Recommendation
[One to two sentences: what to do next based on the tier.]

## Key Evidence
- [Bullet the top 3 facts that drove the score]

## Gaps
- [Bullet what you could not verify or find]
```

## Customization Checklist

Before first use, fill in every bracket placeholder above with your actual targets:
- [ ] Target industries
- [ ] Ideal headcount range
- [ ] Ideal revenue range
- [ ] Target geographies
- [ ] Business model
- [ ] Compatible tech stack
- [ ] Complementary tools

## Anti-Patterns to Avoid

1. **Scoring on firmographics alone.** A perfect-size company with zero intent is not a Tier A lead. Require signals from at least two categories for Tier A.
2. **Treating all signals equally.** A pricing page visit is worth more than a matching geography. Weight accordingly.
3. **Keeping stale scores.** Re-score any prospect that has been sitting for more than 30 days. Triggers and intent decay fast.
4. **Guessing when data is missing.** If you cannot find evidence for a signal, score it zero and note it in the Gaps section. Do not inflate.
