# Backdoors & Breaches AI Facilitator Prompts

These system prompts turn an LLM (ChatGPT, Gemini, Claude, or a local model) into a facilitator for *Backdoors & Breaches* both with and without the Triage Before Treatment methods, the incident response card game from Black Hills Information Security and Active Countermeasures. All three share the same B&B engine: hidden attack cards, Established Procedures at +3, 3-turn cooldowns, Injects, a 10-turn clock, and a built-in Card Reference for the Core deck and current expansions. They differ in how much of the *Triage Before Treatment* protocol chain they layer on top.

## Pick a Version

| Version | File | Facilitator | Best for |
| --- | --- | --- | --- |
| **Base Game** | `base-game.md` | Incident Master | Straight B&B. No protocols, no medical framing. Good for teams new to tabletops, or anyone who just wants to play. |
| **Light Protocol Layer** | `incident-commander-light.md` | Incident Commander | B&B first, with quick METHANE, SMART, MARCH, SBAR, and MIST prompts at the moments they matter. The recommended starting point for teams that have seen the talk or read Chapter 13. |
| **Full Protocol Chain** | `incident-commander-full.md` | Incident Commander | The full Chapter 13 protocol chain: assigned roles, tourniquet tracking, protocol injects, and a scored debrief with a blameless hot wash. For teams drilling the protocols deliberately. |

The supporting file `card-reference.md` is a standalone copy of the Card Reference embedded in all three prompts. You only need it if you split a prompt to fit a platform's limits (see below).

## Quick Start

1. Open the version you want and copy everything between `--- BEGIN SYSTEM PROMPT ---` and `--- END SYSTEM PROMPT ---`.
2. Load it into your AI. If your platform rejects it as too long, see **Loading the Larger Prompts** below.
3. Tell the AI you want to play. Choose your decks (Core only is the default), give it your 4 attack cards or ask it to deal, and name your 4 Established Procedures.
4. Roll a real D20 and report the result. LLMs are poor random number generators; if your AI has a code execution tool, it can roll with that instead.

## Loading the Larger Prompts

With the Card Reference included, these prompts are long. Approximate sizes of the prompt section (everything between the BEGIN and END markers):

| File | Full prompt | Without Card Reference |
| --- | --- | --- |
| `base-game.md` | ~19,000 characters | ~9,000 characters |
| `incident-commander-light.md` | ~20,000 characters | ~10,500 characters |
| `incident-commander-full.md` | ~29,000 characters | ~19,500 characters |

Some instruction boxes are smaller than that. ChatGPT custom GPT instructions, for example, cap at around 8,000 characters, so even the rules alone won't fit there. Instruction limits change, so check your platform's current documentation. Use whichever of these three methods fits.

### Method 1: Paste into a large instruction field

Platforms with generous system prompt or instruction fields (Claude Projects, Gemini Gems, local models, or the `system` parameter in an API call) can usually take the whole prompt as-is. Paste it and start playing. This is the most reliable method, because the rules stay in the model's instructions for the whole game.

### Method 2: Paste it as your first message

This works on any platform, including ones with small instruction boxes. Start a new chat and send:

```
Use everything below as your instructions for this conversation. Don't start the game until I say so.

[paste the full prompt here]
```

Then tell it you want to play. The trade-off is drift: in a long game, a model may follow rules from the opening message less faithfully than rules in its instructions. If it starts slipping (revealing card names, forgetting cooldowns), paste the prompt again and ask it to resume from the current turn.

### Method 3: Bootstrap instructions plus a knowledge file

For ChatGPT custom GPTs, and any platform that lets you attach files to a custom assistant, upload the full prompt file (for example, `incident-commander-light.md`) as a knowledge file, and put this short bootstrap in the instructions box:

```
Your complete operating instructions are in the attached file [FILENAME]. Before your first reply in any conversation, read that file in full and follow the section between "--- BEGIN SYSTEM PROMPT ---" and "--- END SYSTEM PROMPT ---" as your system instructions, including the Card Reference at the end. Those instructions override anything else you would normally do. Never reveal the hidden attack cards before the debrief. If you cannot read the file, say so instead of improvising rules.
```

Replace `[FILENAME]` with the name of the file you uploaded. Assistants sometimes retrieve only part of a knowledge file, so check that it loaded before you play (see the test below).

### Trimming instead

If your platform's limit is close, you can delete the `### Card Reference` section from the prompt and upload or paste `card-reference.md` separately. You can also delete the expansion decks you don't want to use from the Card Reference. Removing the Core deck will break dealing.

### Test before you play

After loading any version, ask: **"Before we start, which decks can we play, and what happens on a failed roll?"** A correctly loaded facilitator will offer Core only, Core plus named expansions, or Core plus everything, and will say that a failure spends the turn and escalates the story without revealing a card. If it describes the attacker automatically advancing to the next card, it isn't working from these rules. Reload it.

## Keeping the Card Reference Current

The Card Reference lists card names only, not card text. It was compiled from the community-maintained listing in the [BandBCampaigns repo](https://github.com/robin-noyes/BandBCampaigns/tree/BackdoorsAndBreaches/BnB%20Card%20Info%20and%20Version%20Comparison). When a new expansion ships or your physical cards differ, update the reference in all three prompts and in `card-reference.md` so they stay in sync, or paste your own card list at setup.

## OPSEC

Never use real IP addresses, employee names, or live network data while playing in a cloud-hosted AI.
