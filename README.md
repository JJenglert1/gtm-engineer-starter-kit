# GTM Skill Pack for Claude Code

Pre-built Claude Code skills for SDRs, marketers, founders, and anyone in a Go-To-Market role who wants to automate their sales workflows — no engineering background required.

---

## What's Inside

This repo ships with 5 ready-to-use skills. Each one is a text file that tells Claude Code how to handle a specific GTM workflow.

| Skill | What It Does |
|-------|-------------|
| **Prospect Research** | Builds a research brief on any target account — company overview, recent news, key people, potential pain points |
| **ICP Scorer** | Scores a lead or account against your Ideal Customer Profile and explains why it's a fit (or not) |
| **Outreach Writer** | Drafts personalized cold emails, follow-ups, and sequences based on your research and ICP |
| **Meeting Prep** | Generates a pre-call brief with talking points, objection handling, and discovery questions |
| **Weekly Pipeline Digest** | Summarizes your deals in plain language — what's moving, what's stuck, and what needs attention |

---

## Quick Start

Follow these steps in order. The whole setup takes about 10 minutes.

**Step 1: Clone this repo (download it to your computer)**
Open Claude Code (desktop app or terminal) and tell it to clone the repo. Cloning just means downloading a copy of these files to your computer.

```
git clone https://github.com/JJenglert1/gtm-skill-pack.git
```

Never used a terminal before? Start with the beginner guide first: **[Learn Claude Code (For Non-Engineers)](https://github.com/JJenglert1/claude-code-for-beginners-tips)**

**Step 2: Open it in Claude Code**
Navigate into the folder. Claude will automatically read the CLAUDE.md file and configure itself for GTM work.

```
cd gtm-skill-pack
```

**Step 3: Customize your ICP**
This is the most important step. Open `templates/starter-icp-template.md`, fill in your details, then tell Claude: "Update the ICP scorer skill using the details in templates/starter-icp-template.md." Or you can edit `skills/icp-scorer/SKILL.md` directly — it's just a text file. Everything else builds on this.

**Step 4: Check out the examples**
Look in the `examples/` folder to see what good output looks like — a sample research brief, outreach sequence, and meeting prep brief that all connect into one workflow.

**Step 5: Run your first research brief**
Ask Claude to research a prospect. Try something like:

```
Research Acme Corp and score them against my ICP
```

**Step 6: Iterate and adjust**
The skills are just text files with instructions. If the output isn't quite right, tell Claude to update the skill, or open the file and tweak it yourself. No code involved.

---

## Folder Structure

```
gtm-skill-pack/
├── README.md                              <- You are here
├── CLAUDE.md                              <- Configures Claude for GTM work
├── skills/
│   ├── icp-scorer/SKILL.md                <- Lead/account scoring against your ICP
│   ├── prospect-researcher/SKILL.md       <- Account research briefs
│   ├── cold-outreach-writer/SKILL.md      <- Cold email and sequence drafting
│   ├── meeting-prep-brief/SKILL.md        <- Pre-call briefs and talking points
│   └── weekly-pipeline-digest/SKILL.md    <- Weekly deal status summaries
├── examples/
│   ├── sample-research-brief.md           <- Example: researching a prospect
│   ├── sample-outreach-sequence.md        <- Example: 3-email sequence
│   └── sample-meeting-prep.md             <- Example: pre-call brief
├── templates/
│   └── starter-icp-template.md            <- Fill-in-the-blank ICP setup
└── prospects/                             <- Your output goes here (gitignored)
    ├── research-briefs/
    ├── outreach-drafts/
    └── meeting-prep/
```

---

## How to Customize

**Start with the ICP Scorer.** This is the foundation. Your ICP criteria flow into research briefs, outreach personalization, and meeting prep. Get this right first.

**Then adjust the other skills to match your voice.** Each skill file has clear sections you can edit:
- **Outreach Writer** — Add your tone guidelines, email length preferences, and example emails that sound like you
- **Prospect Research** — Add the specific data points your team cares about (funding stage, tech stack, hiring signals)
- **Meeting Prep** — Add your product's key value props and common objections
- **Weekly Pipeline Digest** — Define what "at risk" means for your sales process

You don't need to know how to code. These are plain text files with instructions. If you can write a Google Doc, you can customize these skills.

---

## New to Claude Code?

If this is your first time using Claude Code, start with the beginner guide:

**[Learn Claude Code (For Non-Engineers)](https://github.com/JJenglert1/claude-code-for-beginners-tips)** — A step-by-step guide to getting set up, even if you've never opened a terminal.

---

## A Note on Security

Skills are just text files with instructions — but you should still review any skill before you install it, especially if it comes from outside this repo. Read through it first. If something looks unfamiliar, ask Claude to explain what it does before you run it.

---

## Join the Community

Have questions, feedback, or want to share your custom skills? We'd love to hear from you.

- Star this repo to stay in the loop on new skills
- Open an issue if you have questions or want to request a new skill
- Submit a pull request if you build something others could use

---

## Want Help Bringing AI to Your GTM Team?

If you're looking to bring Claude Code or AI transformation to your sales and marketing org, we offer a free AI audit to help you figure out where to start.

**[Book a Free AI Audit with Tenex](https://www.tenex.co/get-started?utm_source=github&utm_medium=repo&utm_campaign=gtm_skill_pack)**

---

Built entirely with Claude Code. No code was written manually.
