# Navajo Girls Fastpitch Rules — AI Skill

Get instant, accurate answers to Navajo Girls Fastpitch (NGF) 2026 league rules questions — with NGF local rules layered on top of USA Softball 2026 Fast Pitch rules, rule citations, division notes, and step-by-step reasoning for complex plays.

> **Not in NGF?** A USA Softball-only version of this skill (no local league rules) is available at [jlaunder/ai-skill-usa-softball-rules](https://github.com/jlaunder/ai-skill-usa-softball-rules).

## What it does

Ask any NGF or Fast Pitch rules question in plain English and get an answer with the same accuracy and authority as a certified umpire. The skill:

- Applies NGF local rules first — where NGF rules differ from USA Softball, the NGF rule governs
- Cites the specific rule number and section in every answer
- Applies Fast Pitch rules only (ignores Slow Pitch variants)
- Notes when a rule differs by division (pitching distance, base path length, ball size, stealing home, etc.)
- Reasons through complex multi-rule situations step by step
- Tells you when the answer isn't in the rules rather than guessing

**Example questions:**

- "Can a runner steal home in 8U?"
- "What ball does 10U use?"
- "How many innings can a pitcher throw in a week in 12U?"
- "What are the TOC mercy rules?"
- "Is an unreported substitute allowed to bat?"
- "What is the infield fly rule and when does it apply in NGF?"
- "What version is this skill?"

---

## What you need

- A [Claude account](https://claude.ai) (free or paid)
- **Code execution enabled** — go to Settings > Capabilities and turn on Code execution. Skills require this to be on.
- The **Claude mobile app** (optional but recommended) — download it on the [App Store](https://apps.apple.com/us/app/claude-ai-assistant/id6473753684) or [Google Play](https://play.google.com/store/apps/details?id=com.anthropic.claude) to have quick access during games.

---

## Installation

1. Go to the [Releases](../../releases) page and download the latest `ngf-softball-rules-skill.zip`
2. In Claude, go to **Customize > Skills**
3. Click **+**, then **+ Create skill**, then **Upload a skill**
4. Upload the zip file

That's it. The skill will appear in your skills list and can be toggled on or off at any time from Customize > Skills. Once installed, your skill is also available in the Claude mobile app.

---

## How to use it

Just ask your question — Claude will automatically recognize softball rules questions and use this skill. You can also invoke it manually by typing `/ngf-softball-rules` followed by your question.

---

## Coverage

| Rules file | What it covers |
| --- | --- |
| NGF Local Rules | Field dimensions, game balls, time/run limits, pitching limits, helmets, cleats, stealing by division, substitutes, TOC rules — all NGF-specific |
| Rule 1 — Definitions | All defined terms |
| Rule 2 — The Playing Field | Field and diamond dimensions |
| Rule 3 — Equipment | Bats, balls, helmets, uniforms, cleats |
| Rule 4 — Players, Coaches, Substitutes | Substitutions, courtesy runners, DP/FLEX, re-entry, blood rule |
| Rule 5 — The Game | Game duration, conferences, short-handed rule |
| Rule 6A — Pitching | Legal delivery, crow hop, leaping, illegal pitches |
| Rule 7 — Batting | Batter's box, strikes, balls, batting order |
| Rule 8 — Batter-Runner and Runner | Base running, stolen bases, interference, obstruction, awards |
| Rules 9–12 | Protests, umpires, scoring, use of rules |
| Rules Supplement #1–55 | Detailed supplemental guidance on 55 specific topics |

---

## FAQ

**Do I need a paid Claude account?**
No. The skill works on a free Claude account.

**Does it work offline?**
No. Claude requires an internet connection. Download the mobile app ahead of time and make sure you have a signal at the field.

**Does it cover Slow Pitch or Modified Pitch?**
No. This skill applies Fast Pitch rules only. Slow Pitch and Modified Pitch variants are intentionally excluded.

**Is this official? Is it endorsed by USA Softball or NGF?**
No. This is an independent tool built from publicly available documents. It is not affiliated with or endorsed by USA Softball or Navajo Girls Fastpitch (NGF). Always defer to your league's official rulebook and Umpire in Chief for final rulings.

**What if it gets a rule wrong?**
See the Report an Issue section below.

---

## Report an Issue

If the skill gives an incorrect or incomplete answer, email [jeremy@jeremylaunder.com](mailto:jeremy@jeremylaunder.com) and include:

- The exact question you asked
- The response you received
- What the correct answer should be (with the rule number if you know it)

---

Sources: NGF Rules and Regulations (Revised March 2026), NGF 2026 Spring TOC Rules, USA Softball 2026 Official Rules of Softball
