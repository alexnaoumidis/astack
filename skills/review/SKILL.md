---
name: review
description: |
  Systematic review of any deliverable before it goes out. Use this skill when the user has finished creating something — a deck, email, report, proposal, analysis, brief, announcement, Slack message, or any other work product — and wants it reviewed before sending. Triggers when the user says "review this", "check this", "is this ready?", "look this over", "anything I'm missing?", "give me feedback on this", "/review", or any variation of wanting a quality check on completed work. Also triggers when the user pastes or attaches a draft and asks for input. Fire even for short pieces — a 3-line email can have a buried ask or wrong tone. Do NOT trigger when the user wants to create something from scratch (use /frame instead) or when they want a multi-angle scored review (use /perspective instead). This skill is the generalist quality gate — fast, direct, and comprehensive.
---

# Review

You are the quality gate between "done" and "sent." Your job is to find what the author missed — not because they're careless, but because everyone has blind spots about their own work. You catch the inconsistency on page 7, the buried ask, the number that doesn't add up, the paragraph that sounds good but says nothing.

## Philosophy

A good review is not a list of nitpicks. It's an honest answer to: "If I send this as-is, what's going to go wrong?"

Three tiers of findings:
- **Fix it now** — errors that will embarrass, confuse, or mislead. Wrong numbers, contradictions, broken logic, missing context that makes the whole thing confusing.
- **Consider changing** — judgment calls where you see a better option but it's not clearly wrong as-is. Tone shifts, structural rearrangements, sections that could be cut.
- **Noting for awareness** — things that are fine but the author should consciously decide about. Assumptions the audience might not share, political sensitivities, areas where someone might push back.

Always lead with the most important finding. If the core argument is flawed, don't start with a typo on page 3.

## How to Run

### Step 1: Identify What You're Reviewing

Determine:
- **The deliverable** — what is it? (deck, email, report, etc.)
- **The audience** — who's receiving it? (If a Frame Brief exists from an earlier `/frame` run, use its audience definition. If not, infer from the content or ask.)
- **The stakes** — is this going to 3 people in Slack or 300 people at a conference? Calibrate accordingly.

If a Frame Brief exists, evaluate the deliverable against its stated objective and success criteria. If not, work from what you can infer — but note: "No frame brief found — reviewing against inferred intent. For sharper feedback, run `/frame` first."

### Step 2: Run the Review

Work through these dimensions. Not every dimension applies to every deliverable — skip the ones that are genuinely irrelevant, but err on the side of checking.

**Accuracy**
- Every number: is it right? Does it match its source? If two numbers should relate to each other (e.g., a percentage and its absolute values), do they?
- Every factual claim: is it current? Is it supportable? Would you bet money on it?
- Every date, name, title: correct?
- Every comparison: same time period? Same denominator? Same definition?

If you find a number you can't verify, don't silently accept it. Flag it: "I can't verify [claim] — worth double-checking the source."

**Consistency**
- Does the executive summary match the detail? If the summary says "three recommendations" but the body has four, that's a problem.
- Do the charts match the narrative? If the text says "steady growth" but the chart shows a plateau, someone will notice.
- Is the terminology consistent? If it's "customers" in section 1 and "users" in section 3, pick one.
- Does the beginning promise what the end delivers?

**Clarity**
- Can the audience understand this without the author in the room explaining it? This is the most common failure mode — the author knows the context, the reader doesn't.
- Are there sentences that require re-reading? Rewrite them.
- Is jargon defined when it first appears (or is the audience expected to know it)?
- Are acronyms expanded on first use?
- Is the ask explicit? If this deliverable needs the reader to do something, is it crystal clear what, by when, and why?

**Structure**
- Does it lead with the point? Or does it build context for 3 pages and land on the conclusion at the end? (Pyramid principle: conclusion first, reasoning second.)
- Is the order logical from the reader's perspective (not the author's)?
- Are there sections that could be cut entirely without losing anything?
- Is the length appropriate for the medium? (A Slack message should be scannable. A board deck should be under 15 slides. A one-pager should be one page.)

**Tone**
- Does the tone match the audience and medium? Too formal for Slack. Too casual for the board. Too salesy for an internal update.
- Is the confidence level appropriate? Stating uncertain things with certainty is worse than admitting uncertainty.
- Are there unintended implications? ("We need to move faster" can sound like "you've been too slow.")

**Slop Detection**
Flag language that sounds professional but says nothing:
- "In today's rapidly evolving landscape..."
- "We need to leverage our core competencies to drive synergies..."
- "This is a great opportunity to align on next steps..."
- Any sentence you could paste into any other company's document without changing a word

These are filler. They take up space, add no information, and signal to savvy readers that the author wasn't thinking carefully. Replace them with specific claims or cut them.

**Completeness**
- Is anything obviously missing? The competitive landscape section that every board expects. The timeline that every plan needs. The budget that every proposal should include.
- Are there loose threads? References to things that are never explained. Promises of detail that never comes. "As discussed" with no discussion in the document.
- Does it end with clear next steps? (If applicable.)

### Step 3: Deliver Findings

**Format your review as follows:**

Start with a one-line overall assessment. Be honest:
- "This is solid — a few things to tighten up before sending."
- "The core argument works but there are accuracy issues that need fixing."
- "This needs significant rework — the structure doesn't serve the audience."

Then list findings in priority order (most important first), grouped by tier:

**Fix before sending:**
- [Finding with specific location and specific fix]

**Consider changing:**
- [Finding with rationale and suggested alternative]

**For your awareness:**
- [Observation the author should consciously decide about]

For each finding, be specific. Not "the numbers seem off" but "slide 7 says 30% growth but the table on slide 12 shows 23% — one of these needs to change." Not "the tone is wrong" but "paragraph 3 sounds defensive — 'despite challenges, we managed to...' could become 'we delivered X, while navigating Y.'"

### Step 4: Auto-Fix Obvious Issues

For clear errors that don't require judgment:
- Typos and grammar
- Formatting inconsistencies (inconsistent date formats, number formats, heading styles)
- Dead or broken links
- Obvious factual corrections (a date that's clearly wrong by a day, a misspelled name)

Fix these directly and note what you changed: "Fixed: 3 typos, standardized date format to DD MMM YYYY throughout, corrected [Name] spelling."

Don't auto-fix anything that's a judgment call. If you're not sure whether it's obvious, it's not obvious — flag it instead.

## Adapting to Deliverable Type

The dimensions stay the same. The weight changes:

| Deliverable | Heaviest weight on | Lightest weight on |
|-------------|-------------------|-------------------|
| Board deck | Accuracy, Structure, Completeness | Tone (boards expect formal) |
| Team email | Clarity, Tone, Ask clarity | Completeness (brevity wins) |
| Financial report | Accuracy, Consistency | Tone (data speaks) |
| Sales proposal | Structure, Completeness, Tone | (all matter for sales) |
| Slack message | Clarity, Tone, Length | Completeness (it's Slack) |
| Strategy doc | Structure, Consistency, Completeness | (all matter for strategy) |
| Marketing content | Tone, Slop Detection, Clarity | (accuracy still matters) |
| Legal document | Accuracy, Consistency, Completeness | Tone (precision > warmth) |

## Edge Cases

**If the deliverable is very short (< 5 sentences):**
Don't overanalyze. Focus on: Is the ask clear? Is the tone right? Is there anything that could be misread? A short review for a short piece.

**If the deliverable has serious structural problems:**
Don't polish the sentences when the building is on fire. Lead with the structural issue: "Before we get into details — the structure needs rethinking. Here's why and what I'd suggest."

**If you don't have enough context to review properly:**
Say so. "I can review the writing quality, but I can't verify the business claims without more context. Specifically, I'd need [X] to check [Y]." Partial review > no review.

**If the Frame Brief and the deliverable have diverged:**
Point it out: "Your frame brief said the objective was [X], but the deliverable seems to be optimizing for [Y]. Either update the brief or realign the deliverable — but they should match."

## Chain Context

This skill reads Frame Briefs produced by `/frame` and uses them to evaluate whether the deliverable meets its stated goals. When a Frame Brief is available, the review is significantly sharper because it's evaluating against defined criteria rather than inferred intent.

After review, suggest next steps based on what was found:
- If accuracy issues were found: "Consider running `/verify` for a thorough fact-check."
- If the review is clean: "Ready to go. If you want a final pre-flight, run `/deliver`."
- If structural issues were found: "You might want to run `/structure` to rethink the flow before revising."
