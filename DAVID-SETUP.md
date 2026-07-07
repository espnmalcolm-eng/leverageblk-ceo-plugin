# LeverageBLK CEO plugin — David's setup guide

Hey David — this is your Claude setup. Install it once and Claude shows up to every
Cowork session already knowing the company, brand voice, and how to hand work to Malcolm.

---

## Step 1 — Install Cowork

Download Claude Desktop from https://claude.ai/download and open the Cowork tab,
or go directly to https://claude.ai/cowork

---

## Step 2 — Connect Gmail

In Cowork, open Settings → Connectors → search "Gmail" → connect with the
leverageblk@gmail.com Google account. This is how briefs reach Malcolm.

---

## Step 3 — Install the plugin

In a Cowork session, run:

```
/plugin install https://github.com/espnmalcolm-eng/leverageblk-ceo-plugin
```

Once installed, Claude knows everything it needs — no setup every session.

---

## What you can do

| Command | What it does |
|---|---|
| `/brief <ask>` | Turns your ask into a structured brief and sends it to Malcolm |
| `/content <ask>` | Drafts on-brand copy, posts, or outreach in LeverageBLK's voice |
| `/sync` | Gives you a CEO-readable summary of what's shipped and what's coming |

---

## How the brief loop works

1. You describe what you need — bug, feature, copy change, landing page update
2. Claude writes a structured brief (you approve it first)
3. Brief goes to leverageblk@gmail.com automatically
4. Malcolm's Claude Code picks it up at his next session, runs it, replies to the thread
5. You see the reply in Gmail — what changed, what to check

**Landing page asks** go to the web team. **App asks** go to the mobile build.
Claude knows which is which and asks if it's not obvious.

---

## One rule

Always use `/brief` for anything product or engineering — never send a vague ask directly.
A clean brief means Malcolm's agents can act without a back-and-forth.

Questions → leverageblk@gmail.com or text Malcolm.
