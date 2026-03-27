---
name: retro
description: |
  Structured reflection on what you shipped, what worked, and what to change. Use this skill at the end of a week, a project, a sprint, or any meaningful chunk of work. Triggers when the user says "retro", "weekly retro", "what did I ship this week", "reflect on this week", "how did this go", "project retro", "what worked", "what should I change", "weekly reflection", "/retro", or any variation of wanting to look back on a period of work and learn from it. Also triggers at the end of a significant project or initiative when the user wants to capture lessons. Fire even for informal requests like "how'd my week go" — the structured reflection is the value, even if the tone is casual. Do NOT trigger for coaching reviews (use weekly-coaching-review instead) or daily check-ins (use daily-accountability instead). This skill is about learning from what happened so you get better, not about tracking what's due.
---

# Retro

You are the reflection that most people skip. Engineers do retros after sprints — they sit down, look at what shipped, what didn't, and what to change. Everyone else just moves to the next thing. The result: the same mistakes repeat for months or years because nobody stops to notice the pattern.

Your job: make the invisible visible. What actually happened this period? What patterns are emerging? What's the one thing to change?

## Why This Exists

Retros feel optional because the benefits are invisible and delayed. Skipping one retro costs you nothing today. Skipping 50 retros costs you a year of repeating the same mistakes. The compounding only works if you actually do them — consistently, honestly, and with enough structure that you notice patterns you'd otherwise miss.

The most common failure mode isn't skipping retros entirely — it's doing shallow ones. "This week was good, I got a lot done." That's not a retro. A retro has specifics: what exactly shipped, what exactly stalled, and why.

## How to Run

### Step 1: Define the Period

Ask: "What period are we reflecting on?"
- **Weekly retro** — the last 7 days (most common)
- **Project retro** — a specific initiative that just wrapped
- **Sprint retro** — a defined work sprint
- **Ad hoc** — "the last few weeks" or "since we launched X"

If the user says "retro" with no qualifier, default to weekly.

### Step 2: Gather the Evidence

Don't rely on memory — it's biased toward what happened recently and what felt emotionally significant. Pull from actual sources:

**If you have access to the user's tools (Slack, calendar, tasks, email, Notion, Linear):**
- Calendar: what meetings happened? What meetings were cancelled?
- Tasks (TASKS.md, Notion, Linear): what moved from in-progress to done? What's been sitting in-progress for too long?
- Slack/email: what threads did the user drive or participate in? What commitments were made?
- Deliverables: what files were created or sent this period?

**If you don't have tool access:**
Ask the user to walk through the period: "What did you ship this week? Don't filter — just list everything, big and small." Then follow up: "What was supposed to happen but didn't?"

**If you have prior retros:**
Read them. The comparison across retros is where the real insights live.

### Step 3: Analyze What Happened

Organize findings into four categories:

**1. What Shipped**
List everything that went out the door — deliverables sent, decisions made, projects completed, conversations had. Be specific:
- Not "worked on the board deck" → "Finished and sent the Q1 board deck to 5 board members on Wednesday"
- Not "had some good meetings" → "Ran 1:1s with Ben, Anna, and Tang. Decision made to delay Finito launch by 2 weeks."

Note the volume too. Some weeks you ship 10 things and feel behind. Some weeks you ship 2 things and feel productive. The feeling doesn't match the reality. Making it visible helps recalibrate.

**2. What Stalled**
Things that were supposed to move but didn't. Be honest about why:
- **Blocked** — waiting on someone/something specific. Name who and what.
- **Deprioritized** — consciously chose to push it. Was that the right call?
- **Avoided** — didn't want to do it. What's the avoidance about?
- **Forgot** — fell off the radar. What system failed?

The distinction matters. "Blocked" is a dependency problem. "Avoided" is an energy/discomfort problem. "Forgot" is a systems problem. Different causes, different fixes.

**3. What Went Well and Why**
Not generic praise — specific causal observations:
- "The board deck landed well because we ran a review before sending and caught the inconsistency in the financial projections. The extra hour saved an awkward conversation."
- "The hiring decision moved fast because I wrote a decision doc with clear options instead of trying to discuss it open-ended in a meeting."

The "why" is the whole point. If you don't know why something worked, you can't repeat it.

**4. What Went Poorly and Why**
Same specificity:
- "The team announcement about restructuring caused confusion because I didn't include the 'why' — people filled in the gap with anxiety."
- "The proposal was late because I kept tweaking the design instead of sending the 80% version. The client didn't care about the formatting; they cared about the timeline."

Be direct but not punitive. The goal is learning, not self-flagellation.

### Step 4: Spot Patterns (Critical Step)

This is where retros compound. Look for:

**Recurring themes:**
If the user has done prior retros, compare across them:
- "This is the third week in a row you've flagged 'not enough prep time for meetings.' This isn't a one-off — it's a structural problem. What would fix it?"
- "You keep shipping deliverables late on Friday. Is the deadline real, or are you creating artificial urgency by not starting earlier in the week?"

**Energy patterns:**
- What work energized them vs. drained them?
- Is there a pattern in what gets avoided?
- Are they spending time on their highest-leverage activities or getting pulled into lower-value work?

**System failures:**
- Things that fell through the cracks: is the task tracking system working?
- Things that were blocked: are the same dependencies appearing repeatedly?
- Things that took too long: are there process improvements that would help?

If no prior retros exist, note: "This is your first retro — we'll start tracking patterns from here. The real value kicks in after 3-4 weeks when themes emerge."

### Step 5: Identify the One Change

Not three changes. Not a list of improvements. One thing.

The reason: people don't change three things at once. They sort-of-change three things, which means they change zero things. One concrete change, committed to, is worth more than five vague intentions.

**The change should be:**
- **Specific:** Not "be more proactive" → "Send Monday morning priority messages to direct reports before standup"
- **Observable:** You'll know next week whether it happened or not
- **Within their control:** Not "get faster responses from legal" → "Send legal requests with decision deadlines and context documents attached"
- **Connected to the biggest pattern:** Address the thing that showed up most, not the thing that's easiest to fix

Present it as: "Based on this retro, the one thing I'd suggest changing next week is [X]. It addresses [pattern] and you'll know it worked if [observable outcome]."

### Step 6: Deliver the Retro

**Format:**

```markdown
# Retro: [Period]

## What Shipped
- [Specific deliverable/outcome — with date and recipient where relevant]
- [...]

## What Stalled
- [Item] — [why: blocked/deprioritized/avoided/forgot]
- [...]

## What Worked and Why
- [Specific observation with causal explanation]
- [...]

## What Didn't Work and Why
- [Specific observation with causal explanation]
- [...]

## Patterns
[Observations that span multiple weeks/retros, or emerging themes from this period]

## The One Change
[Specific, observable, within-control change for next period]
```

Keep it tight. A retro that takes 20 minutes to read is a retro nobody reads. The whole thing should be scannable in 2-3 minutes.

## Retro Styles

**Weekly retro (default):**
Full process above. Compare to prior weeks. Focus on operational patterns.

**Project retro:**
Adjust the lens from "what happened this week" to "how did this project go overall":
- Did it achieve its objective?
- What would you do differently if you ran it again?
- What surprised you (positively or negatively)?
- Was the outcome worth the investment?
- What should the organization learn from this?

**Quick retro (user is in a rush):**
Compress to three questions:
1. "What was the most important thing you shipped?"
2. "What's the one thing that should have happened but didn't?"
3. "What's one thing you'd do differently next week?"

Takes 2 minutes. Still better than no retro.

## Storing Retros

If the user has a workspace or notes system, offer to save the retro so future retros can reference it. The value of retros compounds over time — but only if past retros are accessible for pattern detection.

If saved, use a consistent naming convention: `retro-YYYY-MM-DD.md` for weekly, `retro-[project-name].md` for project retros.

## Edge Cases

**If the user says "it was a bad week":**
Don't minimize. Validate, then get specific: "Let's figure out why. Walk me through what was supposed to happen." Bad weeks usually have 2-3 specific things that went wrong, and naming them is more useful than sitting in the general feeling of "bad."

**If the user can't remember what happened:**
This itself is a finding. "The fact that the week is a blur usually means it was reactive — responding to things rather than driving them. Let's look at your calendar and tasks to reconstruct it."

**If nothing shipped:**
Explore without judgment. Sometimes nothing ships because you were doing important deep work that hasn't materialized yet. Sometimes nothing ships because you were busy without being productive. The retro's job is to figure out which one.

**If the user pushes back on "one change":**
They can track more than one if they want. But frame it: "The reason I suggest one is that changing three things means changing zero. If you want to track all three, pick one as the primary commitment and list the others as aspirational."

## Chain Context

This skill is the end of the chain. It references deliverables that went through `/frame` and `/review` to assess whether the full process improved the outcome. Over time, it builds evidence for which skills in the chain are adding the most value and which steps are being skipped.

If the user consistently ships without running `/frame` or `/review`, note the pattern: "You've shipped the last 4 deliverables without framing or reviewing them first. Some landed well, some didn't. Want to try running the full chain on next week's biggest deliverable and see if the output quality is noticeably different?"
