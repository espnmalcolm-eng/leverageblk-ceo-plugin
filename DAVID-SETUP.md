# LeverageBLK — David's Claude setup

One-time setup. After this Claude shows up to every session already knowing the
company, brand voice, and how to hand work to Malcolm.

---

## Step 1 — Download Claude Desktop

Go to https://claude.ai/download → download and install → sign in with your account.
Open the app and switch to the **Cowork** tab.

---

## Step 2 — Paste your Global Instructions

Global Instructions load at the start of every Cowork session automatically.

1. In Cowork, go to **Settings → Cowork → Edit** next to "Global instructions"
2. Open the file `GLOBAL-INSTRUCTIONS.md` (in this folder)
3. Copy everything and paste it into the text box
4. Click **Save**

Done. Claude now knows who you are, the brand, and how briefs work — every session.

---

## Step 3 — Connect Gmail

In Claude Desktop: **Settings → Connectors → search "Gmail" → connect**
Use the leverageblk@gmail.com Google account.

This is how briefs reach Malcolm and how you see his replies.

---

## Step 4 — Create your LeverageBLK Cowork Project

Projects give you memory across sessions — Claude remembers what you worked on last time.

1. In Cowork, click **Projects → New Project**
2. Name it: `LeverageBLK`
3. Point it at this folder on your computer (wherever you saved it)
4. Add instructions: paste the contents of `GLOBAL-INSTRUCTIONS.md` here too
5. Click **Create**

Use this project for all LeverageBLK work so Claude builds context over time.

---

## How to use it day to day

**Send Malcolm a brief**
Just describe what you need and Claude will write the structured brief and send it:
> "The waitlist form on the landing page feels slow on mobile, can we fix it?"

Claude will ask a couple of clarifying questions, write the brief, show it to you,
and send it to leverageblk@gmail.com once you say go.

**Draft on-brand content**
> "Write a LinkedIn post announcing the HBCU ambassador program"
> "Draft an outreach email to the NABJ DC chapter"
> "Write Instagram copy for the culture mixer event"

Claude applies the LeverageBLK voice automatically from your global instructions.

**Check sprint state before a call**
> "What's shipped and what's coming? I have a partner call in 20 minutes."

Claude will summarize what Malcolm's side has been working on in plain language.

**Check Gmail for brief replies**
> "Any replies from Malcolm on open briefs?"

Claude reads leverageblk@gmail.com and surfaces what came back.

---

## One rule

Always describe what you need before Claude acts — it will ask clarifying questions
if anything is unclear. That question-first step is what keeps briefs clean and
prevents Malcolm's agents from building the wrong thing.

---

## What each brief type means for Malcolm

| Type | What happens on Malcolm's side |
|---|---|
| `landing` copy or design | Goes to the web repo, runs as a build loop |
| `app` bug or feature | Goes to the mobile repo, Codex executes it |
| `infra` | Goes to Supabase, database-level work |
| `p0` | Malcolm sees it immediately — blocking |
| `p1` | This sprint — picked up at next session start |
| `p2` | Backlog — queued for later |

---

Questions → text Malcolm or reply to any email in the leverageblk@gmail.com thread.
