# Business Data

This folder is where your **real business information** lives. The agents read it and treat it as **evidence**. Anything not backed by these files gets labeled as inference.

Without this folder, the agents can only guess from `business-brief.md`. With it, they work from what your buyers actually say and do.

---

## ⚠️ Privacy first: this GitHub project is PUBLIC

Anyone on the internet can read files that get uploaded to GitHub from this project.

- **Anonymize everything** in the files below. Write "Client A, coach, 2 years in business," not a name, email, or company.
- **Anything with real names, emails, or raw exports goes in `data/private/`.** That folder is never uploaded (a file called `.gitignore` blocks it). The agents can still read it on your computer.
- **Want full privacy?** On GitHub, open the project → **Settings** → scroll to **Danger Zone** → **Change visibility** → **Private**.

---

## What goes where

| File | What to put in it | Where it comes from | Time |
|---|---|---|---|
| `audience-poll.md` | Poll question, answer options, vote counts | A YouTube community post, Instagram story, or email | 10 min to post |
| `buyer-language.md` | Exact words buyers use about their problems | DMs, emails, discovery call notes, comments, testimonials | 20 min |
| `channel-analytics.md` | Your top videos and the search terms people use to find you | YouTube Studio → Analytics | 15 min |
| `offers-and-pricing.md` | What you sell today, what it costs, who buys it | You | 10 min |
| `relay-test-log.md` | Results of each control-prompt vs. Relay test run | You, after running the go/no-go test | 5 min per test |
| `private/` | Raw exports, call transcripts, anything with real names | Anywhere | — |

**You don't need everything at once.** Start with `audience-poll.md` and `buyer-language.md`. Those two fix the biggest gaps the researcher found.

---

## How to use it

1. Fill in one or more files. Replace the `[brackets]` and delete the example rows.
2. Open this project in Claude Code and say: *"Follow the runbook. Use the data folder as evidence."*
3. The researcher will label claims as **[Data]** (from these files), **[Brief]**, **[Inference]**, or **[Unknown]**. More [Data] labels means a stronger video.

**Golden rule: paste, don't paraphrase.** Buyers' exact words are worth more than your summary of them.
