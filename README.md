# Triage Before Treatment: Tabletop Kit

Everything here comes from the talk *Triage Before Treatment: Running Incident Tabletops Like a Trauma Bay*, first given at Triangle InfoSeCon on 30 October 2026 and is provided as a jumpstart to your own tabletops. .

This repo, and everything else on this GitHub is for the betterment of the (SMB) community. Some of it works for enterpise too. Take it, change it, run it.

## The method

A trauma bay works on two ideas, and so does this kit.

**Order.** One incident commander. Everyone reports to them. Find what's killing the business before you fix anything. Triage before treatment.

**Clear updates.** Going up, a structured escalation instead of a ramble. Going across, a handoff that says exactly what you already changed.

Everything in this kit serves one of those two ideas.

## Borrowed, not invented

Every tool in this kit is already in use by people who handle more "worse days" than most of us. As security practitioners that is "ugh, ransomware". As operational and emergency medical professionals,it's a lot different. None of it was invented for this talk.

| Tool | What it is | Where it comes from | What it does here |
|---|---|---|---|
| **ICS** | Incident Command System | Fire service | One commander. Everyone reports up. |
| **START** | Mass-casualty triage | EMS and fire | Sort before you treat, in four colors |
| **SBAR** | Situation, Background, Assessment, Recommendation | Navy submarines, then hospitals | How you escalate to the person who decides |
| **MIST** | Mechanism, Injuries, Signs, Treatment | Military and EMS trauma handoff | What you hand the next team |

You don't need a new framework. You need to steal one that already works under pressure.

## What's here

| File | What it is |
|---|---|
| [`kestrel-scenario.md`](kestrel-scenario.md) | The Kestrel Manufacturing scenario, all six injects, and facilitator notes for each |
| [`triage.md`](triage.md) | The four triage categories for assets, and a triage sheet |
| [`sbar.md`](sbar.md) | SBAR for escalating to executives, with a worked example |
| [`handoff.md`](handoff.md) | The MIST handoff sheet: mechanism, injuries, signs, treatment given |
| [`hot-wash.md`](hot-wash.md) | A hot wash template that ends with an owner on every finding |

## Run it next month

1. Read `kestrel-scenario.md` once, start to finish. That's your prep.
2. Share `sbar.md` with whoever will play the incident commander.
3. Pick a format: call and answer with a whole room (15 minutes), or a seated team (30 to 45 minutes). Both are in the scenario file.
4. Run it. Keep the clock moving. Don't rescue anyone.
5. Hot wash within the hour. Every finding leaves with a name on it or NOTHING.

Then do it again next quarter with your own systems swapped in.

## Five rules for running your own

1. **Name an incident commander before the clock starts.** Order has to start with someone.
2. **Every escalation is an SBAR.** The update is the thing being rehearsed.
3. **More red tags than hands.** Without scarcity, nobody has to choose.
4. **Someone new arrives mid-crisis** and asks what you changed.
5. **Debrief while it's fresh.** Every finding leaves with an owner.

## Steal this Monday

Three things. No budget. No permission.

1. **Name your incident commander** before you need one, and write it down where people can find it at 06:40.
2. **Make every escalation an SBAR:** situation, background, assessment, and what you need from them.
3. **Write down every change** you make during an incident. That list is the T in MIST.

## License

Licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Use it at work, adapt it for your clients, teach with it. If you publish a modified version, credit the original and share yours under the same terms.

Steven Lorenz · [stevenlorenz.dev](https://stevenlorenz.dev) (but more of my relevant stuff is on GitHub)
