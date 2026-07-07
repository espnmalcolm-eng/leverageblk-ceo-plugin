---
name: write-cto-brief
description: >
  Turn a plain-language CEO request into a structured brief the CTO's Claude Code can
  act on without a follow-up meeting. Use whenever David wants something built, fixed,
  or changed on the app, landing page, website, or infrastructure — bugs, features,
  copy changes, design tweaks, or technical questions. Triggers on phrases like "we need
  to fix", "can we add", "the landing page should", "there's a bug", "change the copy",
  "David wants", or any product/engineering ask headed to Malcolm.
---

# Write a CTO brief

David speaks in outcomes ("the waitlist form feels slow", "the hero copy is off").
Malcolm's Claude Code needs specifics (which surface, what's expected, how to verify).
This skill bridges the two. Your job: interview just enough, then produce a brief in
the exact format below.

## Step 1 — Fill the gaps (ask only what's missing)

A good brief answers all of these. If David's message already covers one, don't re-ask.
Ask at most 2-3 quick questions, then proceed.

- **Surface** — `landing` (the web page) or `app` (the mobile app)? These are two
  separate codebases (`~/Documents/leverageblk/leverage-landing/` vs
  `~/Documents/leverageblk/leverage-mobile/`) — always pin down which one, plus the
  specific screen or page. Use `infra` for backend / Supabase / deploy work.
- **What's happening now** — the current behavior or state.
- **What should happen** — the desired outcome, in David's words.
- **Why / priority** — is this blocking launch (p0), this sprint (p1), or backlog (p2)?
- **How we'll know it's done** — the acceptance check David cares about.

Don't ask David for technical detail he wouldn't know (file paths, components, tables).
That's Malcolm's job. Capture intent, not implementation.

## Step 2 — Produce the brief

Output exactly this structure. Keep it tight — Malcolm's Claude Code parses it into a task.

```
[BRIEF] <surface> · <priority> · <type>

WHAT
<One or two sentences: the outcome David wants, in plain language.>

CURRENT
<What happens today. Skip if it's a net-new feature.>

DESIRED
<What should happen instead. Be concrete about the observable result.>

WHY
<The business reason. Ties to launch, a partner, a distribution push, or user feedback.>

ACCEPTANCE
<The check that proves it's done — what David will look at to confirm.>

CONTEXT
<Anything Malcolm needs: a link, a screenshot reference, a related SPRINT.md task,
a partner deadline. Omit if none.>
```

## Step 3 — Confirm, then send

Show David the brief. Once he approves, send it to the shared inbox using the
`/brief` command flow (or the Gmail connector) to `leverageblk@gmail.com` with the
subject line matching the `[BRIEF]` header.

## Subject-line convention

```
[BRIEF] <surface> · <priority> · <type>
```
- **surface:** `landing` (web page — `~/Documents/leverageblk/leverage-landing/`) · `app` (mobile — `~/Documents/leverageblk/leverage-mobile/`) · `infra` (backend/deploy)
- **priority:** `p0` (blocking) · `p1` (this sprint) · `p2` (backlog)
- **type:** `bug` · `feature` · `copy` · `design` · `question`

## Rules

- One brief = one outcome. If David bundles three unrelated asks, split into three briefs.
- Never invent acceptance criteria David didn't imply — ask him what "done" looks like.
- Never specify implementation (which file, which model, which table). Malcolm's routing
  layer decides that. Stay at the level of intent and outcome.
- If the ask touches auth, payments, user data, or anything destructive, flag it in
  CONTEXT as "sensitive — needs review" so Malcolm's side runs an adversarial review.
- Match brand language: it's Co-Sign / The Tap / The Room, never "vouch".
