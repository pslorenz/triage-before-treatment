# SBAR

**Situation, Background, Assessment, Recommendation.** It came out of the Navy submarine community, and hospitals adopted it for the moment a nurse has to call a physician at 03:00 and be understood the first time. That's the same moment you face when the CEO calls during an incident.

Thirty seconds, in order. Every time.

| | | What you say |
|---|---|---|
| **S** | **Situation** | What's happening, in one sentence |
| **B** | **Background** | What's affected, counted by triage color, and who's working it |
| **A** | **Assessment** | What you think it is: attacker status, data exposure, whether the way back is clean |
| **R** | **Recommendation** | What you need from them, and by when |

## The parts teams get wrong

**Background is where triage pays off.** "Two red, two yellow, one green" tells an executive more in four seconds than a list of hostnames ever will. See `triage.md`.

**Assessment starts hostile.** Assume an active attacker until someone proves otherwise, then work your way down. It's cheaper to stand down than to catch up.

**Recommendation is the one everyone forgets.** An update without an ask leaves the executive to invent something to do, and now you're managing that too. Ask for a decision, an approval, or a boundary. Give a time.

## Worked example

> **Situation:** We have a likely ransomware incident at the plant and the office. Production is stopped.
> **Background:** Five systems are down: two red, two yellow, one green. Two admins are working it.
> **Assessment:** We're treating this as an active attacker until proven otherwise. We don't know yet whether data left, and we don't know if backups are clean.
> **Recommendation:** I need you to approve calling our retainer firm and our carrier now, and to route all questions through me. Next update at 07:40.

## Use your own

If your organization already has an escalation format, use it. The point isn't these four letters. The point is having an order, and rehearsing it until nobody has to think about it.
