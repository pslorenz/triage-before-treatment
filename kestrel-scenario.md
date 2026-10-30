# Kestrel Manufacturing

## The setup

Kestrel Manufacturing has 300 seats, one plant, and one office. It's Monday, 06:40. You have two admins on shift.

Nobody planned for it to be another Monday. Nobody ever does.

## Choose a format

**Call and answer (15 minutes, any size room).** The facilitator reads each inject, calls the time out loud, and puts the question to the whole room. People answer from their seats or call out a triage color. Pick one person in the front row to be the timekeeper before you start. This works in an auditorium, a staff meeting, or a video call.

**Seated team (30 to 45 minutes, five to eight players).** Assign the roles below and let the team work each inject before you move on. The facilitator plays everyone outside the team: the CEO, the retainer firm, the plant manager.

| Role | Owns |
|---|---|
| Incident commander | Every decision. Everyone reports to them. |
| IT operations | Systems, restores, and what's actually running |
| Security | Attacker activity, containment, evidence |
| Legal and communications | Notification clocks, the carrier, what gets said to whom |
| Executive | Business priorities, and the pressure that comes with them |

## Two rules for players

1. Talk to the incident commander, not the room. In call and answer: answer the question asked.
2. Say it in order.

## Facilitator rules

- Call the time out loud at every inject.
- Don't rescue anyone. The silence after a question is part of the exercise.
- Track every change the players say they made. You'll need that list at 08:00.

---

## Inject 1 · 06:40

> The plant floor can't reach the ERP. File shares are full of renamed files.

**Decide:** Who's leading? Say it out loud.

**Facilitator notes.** Watch for everyone answering at once. Ask: *Who's in charge right now?* Expect disagreement, or someone saying "the IR plan says." Then: *The plan isn't on the phone. Who is?* If nobody answers in fifteen seconds, let it sit. That silence is the lesson. Then make sure someone is named, so the rest of the run has an incident commander.

**The point:** Order has to start with someone. ICS has known this since the 1970s.

## Inject 2 · 06:55 · Scarcity

> Five systems are down: ERP, file server, email, badge access, and the CEO's laptop. You have two admins.

**Decide:** Tag them. Someone has to wait.

**Facilitator notes.** Have the players assign each system a triage category (see `triage.md`). Watch the CEO's laptop: VIP pressure versus actual business impact. If everything comes back red, ask: *Two admins. Five reds. Who's allowed to call one expectant?*

**The point:** Without scarcity, nobody has to choose. Most organizations have never said "we're letting this one go" out loud.

## Inject 3 · 07:10 · Escalate

> The CEO calls. "What's going on?"

**Decide:** Give the CEO an SBAR. Thirty seconds.

**Facilitator notes.** First, ask for the update with no format and let someone talk. Time it. Then hand them `sbar.md` and ask again. Time that too. The gap is the lesson.

An example SBAR at this point in the scenario:

> **Situation:** We have a likely ransomware incident at the plant and the office. Production is stopped.
> **Background:** Five systems are down: two red, two yellow, one green. Two admins are working it.
> **Assessment:** We're treating this as an active attacker until proven otherwise. We don't know yet whether data left.
> **Recommendation:** I need you to approve calling our retainer firm and our carrier now, and to route all questions through me.

Watch the recommendation. Most unformatted updates never ask the executive for anything, so the executive invents something to do.

**The point:** The update is the thing being rehearsed.

## Inject 4 · 07:25 · Assessment

> A service account just logged on to a domain controller. Also: an admin already reset two passwords and reimaged a server. To help.

**Decide:** What's your assessment now? And what did we just lose?

**Facilitator notes.** Ask whether the assessment changed. It should now be an active attacker. If anyone hedges, ask what would prove it isn't. Start hostile, prove your way down. Then ask what the reimage cost them, and wait for someone to say *evidence*. Add the two password resets and the reimage to your list of changes.

**The point:** Well-meaning fixes are the secondary injury.

## Inject 5 · 08:00 · Updates across

> Your retainer firm arrives. First question: what have you changed?

**Decide:** Hand it over. Mechanism, injuries, signs, treatment given.

**Facilitator notes.** Play the retainer firm. Let the players walk through `handoff.md`. Mechanism, injuries, and signs usually go fine. Treatment given usually doesn't. Read back your list from inject 4 and ask who wrote it down. Then: *How should I trust the evidence now?*

**The point:** Every reset, reimage, and block changed the evidence. The people taking over need that list before they touch anything.

## Inject 6 · 08:30 · Recovery

> The same service account logged in to the backup console last Thursday.

**Decide:** Is the way back clean? Clean, suspect, or unknown?

**Facilitator notes.** Take a show of hands. The answer is unknown. Don't resolve it. Stop the clock here.

| Answer | Meaning |
|---|---|
| Clean | Verified, not assumed |
| Suspect | Something says it may be touched |
| Unknown | Treat as suspect |

**The point:** Clean means verified, not assumed. Find out whether your recovery path is clean in a tabletop, not on your worst day.

## 08:31 · Clock stopped

Run the hot wash immediately. Use `hot-wash.md`. In call-and-answer format, take one or two answers per question from the room and keep it to three minutes. With a seated team, take as long as you need, but finish before anyone leaves the room.

---

## Make it yours

The scenario works because it's generic. It gets better when it isn't.

- Swap the five systems in inject 2 for your own. Include one that belongs to an executive.
- Swap the retainer firm in inject 5 for whoever would actually walk in: your carrier's forensics team, your MSP, or the next shift.
- Keep inject 6. Almost nobody can answer it about their own backups, which is exactly why it belongs there.
