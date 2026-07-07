# LeverageBLK CEO plugin

The CEO-side companion to the CTO's `CLAUDE.md`. Install once into Cowork and David's
Claude shows up already knowing the company, the brand voice, and how to hand work to
Malcolm — no re-briefing every session.

## What's inside

- **`CEO-CONTEXT.md`** (repo root) — the master context: company, brand system, sprint
  pointer, distribution lanes, and the CTO handoff protocol.
- **`skills/write-cto-brief`** — turns a plain-language ask into a structured brief
  Malcolm's Claude Code can act on without a meeting.
- **`skills/brand-voice`** — applies LeverageBLK's voice and visual system to any
  public-facing content.
- **`commands/brief`** — `/brief <request>` → structured CTO brief, sent to the shared inbox.
- **`commands/content`** — `/content <ask>` → on-brand copy or asset.
- **`commands/sync`** — `/sync` → CEO-readable summary of current sprint state.

## Install (Cowork / Claude Code)

```
/plugin install leverageblk-ceo
```

Or point the plugin marketplace at this folder / its git location, then install by name.

## How David uses it day to day

- Needs something built or fixed → `/brief the waitlist form feels slow on mobile`
- Needs a post or outreach → `/content LinkedIn post announcing the HBCU ambassador program`
- Prepping for a call → `/sync` before talking to a partner
- Anything public → the `brand-voice` skill runs automatically

## Keeping it current

Malcolm maintains `CEO-CONTEXT.md`. After a feature ships, update `SPRINT.md` — the
`/sync` command reads it live, so David is always working from the same reality without
a standup. The trust-mechanic names (Co-Sign, The Tap, The Room) and the palette/type
canon are locked; change them only when the product does.
