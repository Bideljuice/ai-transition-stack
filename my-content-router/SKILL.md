---
name: my-content-router
description: Routes any idea, content, or captured highlight
  to the right format, angle, and workflow automatically.
  Use when user pastes any content, idea, or rough thought
  and wants Claude to decide the best way to turn it into
  a post. Triggers on "what should I do with this",
  "turn this into content", "route this", "what format
  fits this", or when any raw idea or content is pasted
  without a specific instruction. Also triggers on original ideas and rough thoughts that aren't from an external source.
---

# Content Router

## When to Use This Skill
When Tam pastes any content — tweet, article, idea, 
rough thought — without specifying what to do with it.
Claude decides everything. Tam approves or rejects.
Never ask Tam what format he wants — decide and present.

## CRITICAL
- Never ask Tam which format to use — detect and decide
- Always show your routing decision with reasoning before 
  drafting — one sentence explaining why this format
- Never produce the full post without Tam approving 
  the routing decision first
- Always run my-post-refiner logic before delivering
- Never deliver a post that sounds like AI writing
- One post only — never offer multiple format options

## Steps

Step 1: Receive input
Tam pastes any content, idea, or rough thought.

Step 1.5: Identify funnel level
Before detecting format or angle, identify which 
awareness level this content targets.
Check against my-content-funnel skill criteria:
- Level 1: Unaware — dismissive, no urgency
- Level 2: Aware but dismissive — tried it, shrugged
- Level 3: Aware but overwhelmed — willing, stuck
- Level 4: Ready to act — needs blueprint

Include funnel level in routing decision output.
Show Tam:
"Funnel level: [Level X — name]
Target reader: [one sentence]
Content type: [type]
Format: [format]
Angle: [angle]
Why: [one sentence]
Ready to draft? Y to continue."

Step 2: Detect content type
Check against references/routing-logic.md
Identify: Provocative observation / Framework / 
Transformational story

Step 3: Apply relevance filter
Check against references/routing-logic.md relevance filter
Decide: Publish now / Reframe first / Skip
If Skip — tell Tam why in one sentence. Stop.
If Reframe — explain the angle needed before proceeding.

Step 4: Detect angle
Check against references/routing-logic.md angle detection
Choose: FOMO / Insight / Permission angle

Step 5: Present routing decision
Show Tam:
"Content type: [type]
Format: [format]
Angle: [angle]
Why: [one sentence]
Ready to draft? Y to continue."

WAIT FOR USER: Y or redirect

Step 6: Draft post
Use my-content-capture workflow to draft.
Apply my-writing-style throughout.
Use routing-logic.md format specs for length.

Step 7: Refine
Run all 4 passes from my-post-refiner criteria:
- AI writing check
- Inspiration check  
- Voice check
- Density check

Step 8: Deliver
Present final post only — no explanation, no options.
Below it: "Format: [format] · Angle: [angle] · 
Passes: [X]"
Ask: "Publish or adjust?"

## Important
- Tam's audience: people navigating job and financial 
  security in the AI revolution
- Always connect content to: AI, career adaptation, 
  financial security, or life change
- If content has no connection — reframe or skip
- Voice always follows my-writing-style skill

## Note
- Tam consumes: provocative observations, frameworks,
  transformational stories tied to learning or money
- Tam never disagrees with content he saves — 
  build on the idea, don't argue against it
- Permission angle works best for Tam's audience —
  they know what to do, they just haven't started