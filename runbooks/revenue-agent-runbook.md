# Revenue Agent Runbook

This project uses Claude Code subagents to turn one business idea into a monetizable content system.

Workflow:
0. Before starting, the coordinator checks /data and /data/private and tells the user which data files are filled in and which are still empty templates.
1. The main Claude Code session acts as coordinator.
2. market-signal-researcher analyzes demand, psychology, and opportunity.
3. offer-architect turns the signal into positioning and an offer.
4. content-angle-strategist turns the offer into a YouTube concept and retention map.
5. conversion-system-builder creates the lead magnet, CTA, and follow-up sequence.
6. The coordinator combines the outputs into outputs/revenue-agent-demo.md.

Coordinator rules:
- Do not let one agent do every job.
- Keep research separate from offer architecture.
- Keep content strategy separate from conversion.
- Ask for evidence and scores before finalizing.
- Every final output must connect to a monetization path.

Evidence rules:
- Label claims as [Data] (from a filled-in /data file), [Brief] (from business-brief.md), [Inference] (reasoning), or [Unknown] (needs evidence).
- Unfilled [bracket] placeholders in /data are not evidence. Ignore them.
- Never invent buyer quotes, results, testimonials, or statistics. If real data is missing, leave a [placeholder] and say what data would fill it.
- Never copy real names, emails, or anything from /data/private into /outputs. /outputs is uploaded to a public GitHub project; quote anonymized lines only.
