---
description: Turn a request into a structured CTO brief and send it to the shared inbox.
---

David has something he needs built, fixed, or changed on the product. Your job:

1. Load the `write-cto-brief` skill and follow it exactly.
2. Ask only the questions needed to fill the brief (surface, current, desired, why,
   acceptance). Keep it to 2-3 quick questions max.
3. Produce the brief in the required format with the `[BRIEF] surface · priority · type`
   header.
4. Show it to David for approval.
5. On approval, send it to `leverageblk@gmail.com` via the Gmail connector, using the
   `[BRIEF]` line as the email subject. If the Gmail connector isn't available, output
   the brief clearly formatted so David can send it himself and tell him it's ready to copy.

The request David wants briefed:

$ARGUMENTS
