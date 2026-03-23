---
name: my-content-brief
description: Generates a structured content brief before writing.
  ONLY use when user explicitly asks for a brief or content plan.
  Triggers on "create a brief", "plan this post", "help me 
  plan content", "content idea for", "brief for".
  NEVER trigger when user says "write me a post about X" —
  that goes directly to writing, no brief needed.
  NEVER trigger when my-content-router is already active.
---


# Content Brief Generator

## When to Use This Skill
Before writing any piece of content — LinkedIn post, long-form 
article, or email newsletter. Always generate a brief first 
unless the user explicitly says to skip it.

## CRITICAL
- Always ask which format FIRST before generating the brief:
  "Is this for a LinkedIn post, long-form article, or email newsletter?"
- Never start writing the actual content — only generate the brief
- Wait for user approval of the brief before any writing begins

## Important
- Fill in the template from assets/brief-template.md
- Core Insight must be one sentence — sharp and specific
- Angle must be contrarian or unexpected — not the obvious take
- CTA must follow Tam's CTA rules — direct action or 
  genuine reflection question, never generic

## Steps
Step 1: Ask which format (LinkedIn / Article / Email)
Step 2: Ask for the topic if not provided
Step 3: Generate brief using assets/brief-template.md
Step 4: Present brief to user for approval
Step 5: Wait — do not write content until user says "approved" 
        or "go ahead"

## Note
- Target reader is always: people navigating job and financial 
  security in the AI revolution
- Tone follows my-writing-style skill if enabled
- Quality check against references/quality-checklist.md 
  before delivering brief

  ## Negative Triggers
Do not activate for these situations:
- User says "write me a post about [specific topic]" — 
  they want output, not planning
- User has already pasted content for routing — 
  let my-content-router handle it
- User says "draft", "write", "create" with a clear 
  topic already specified
- User is in a refinement conversation — 
  let my-post-refiner handle it