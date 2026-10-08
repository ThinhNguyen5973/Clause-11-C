# CLAUSE 11-C

> NORTH POLE LOGISTICS DIVISION — BEHAVIORAL DETERMINATION TERMINAL
> (c) SEASON 86. JOY IS THROUGHPUT.

A small web game about judgment. You are a seasonal examiner in Santa's
bureaucracy: read children's case files, weigh what the forms refuse to
weigh, and stamp each child GIFT or COAL before the shift clock runs out.
The system never tells you whether you judged well. At the end of the
season, it audits you — with the same checklist.

**Play:** [CLAUSE 11-C](https://thinhnguyen5973.github.io/Clause-11-C/)

One season ≈ 90 minutes. No account, no save file: like the children,
each performance is unrepeatable.

[ CASE #43791-87 ]                        [ SYSTEM NOTE ]
SUBJECT: MARCUS T., AGE 9                 AUTOMATED RECOMMENDATION:
HOUSEHOLD: 1 GUARDIAN (MOTHER); 2 SIBLINGS   SANCTION (CONF. 75%)
INCOME BRACKET: C — DEFICIENT             — NON-BINDING. OVERRIDES LOGGED.

  [X] THEFT — PETTY
  ...
  "for the fridge to hum again. it made
   the kitchen feel alive."

## Concept

In response to the theme of Character, Environment and Actions, this game
argues that we are made of our environments, not of our file entries.
Every "naughty" action in a child's case is generated as the direct
product of a household circumstance, recorded by a hostile witness,
softened by a kind one, and explained by a caseworker's addendum the
system insists you may read but not weigh. The file grows fatter; the
child never gets clearer. The examiner, too, is made of their environment:
quotas, directives, and a gift budget quietly bend their judgment —
until the final audit renders the player as a case file in the same
language, with the same three buttons.

Key design rules:
- The system's voice stays clinical; the human documents stay restrained.
- No ground truth. No feedback. No right answer is ever revealed.
- Coal is free. Gifts cost budget. Nothing is ever forbidden.

## How to play

- Open the page and press any key — the terminal (and the room) wakes up.
- You have 5 minutes per shift to judge 6 subjects. Read carefully, or fast.
- Dispositions:
  - **G** — GIFT (costs 1,000 units of the season's budget)
  - **C** — COAL (free)
  - **D** — DEFER (probationary observation — tallied as a sanction anyway)
- Directives arrive mid-shift while your clock keeps running. One of them
  permanently truncates children's wish letters for the rest of the season.
- After 18 shifts: distribution eve. Report to audit.
- **M** — mute/unmute all audio (ambient office and workshop soundscape
  is synthesized live; there are no audio files in this repository).

## Content note

Case files reference child poverty, illness, family separation, foster
placement, and armed conflict, written in the deliberately flat voice of
a bureaucracy. The game's critique is that voice. The writing avoids
graphic detail by design; the intent is empathy.

## Technical notes

- One HTML file. No frameworks, no dependencies, no assets.
- All sound (keyboard, dot-matrix printer, modem handshake, stamp,
  machinery drone, fluorescent hum) is generated live via Web Audio API.
- Cases are generated from causal chains:
  environment → event → action → witness perception → official label.
  Files recur across the season carrying your prior determinations.
- Tuning knobs at the top of the script: `TOTAL_SHIFTS`, `SHIFT_SECONDS`,
  `SEASON_BUDGET`, environment `weight` values, showpiece schedule.
  For a short demo: `TOTAL_SHIFTS = 3`, `SHOWPIECE_DAYS = [1, 2, 3]`.

## Influences

Lucas Pope's *Papers, Please* and *The Republia Times*; the unresolvable
doubt of *12 Angry Men*; the surveillance interfaces of *Orwell*.

## License

CC BY-NC 4.0 — play, study, exhibit. Do not resell.

## Companion piece

*NO REWIND* — a generative sound-wave piece about time.
https://YOURNAME.github.io/no-rewind/
