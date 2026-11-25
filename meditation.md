---
title: Meditation
description: Faster mana regeneration, the meditative trance, and how armor slows it
published: true
date: 2026-11-25T13:41:30.441Z
tags: 
editor: markdown
dateCreated: 2026-11-24T08:17:41.202Z
---

# Meditation
Meditation is the skill of restoring mana. It speeds up mana regeneration at all times, and using the skill puts the character in a trance that regenerates mana twice as fast. It also strengthens [Reactive Armor](/reactive_armor) and [Protection](/protection).

## Mana Regeneration
A character regains `1` mana at a time. The delay between points depends equally on Intelligence and Meditation:

`Points = (Intelligence + Meditation) / 2`

`Delay = 7 - 239 * Points / 2400 + 19 * Points * Points / 48000` seconds

The delay is `7` seconds with no Intelligence or Meditation, and `1` second at `100` in both. [Armor](/armor) adds to it, and a trance halves it. It's never shorter than `0.5` seconds or longer than `7`.

With `100` Intelligence and no armor:

| Meditation | Delay (s) | Delay in Trance (s) | Mana per Minute | Mana per Minute in Trance |
|:-|:-:|:-:|:-:|:-:|
| 0 | 3.01 | 1.51 | 20 | 40 |
| 25 | 2.32 | 1.16 | 26 | 52 |
| 50 | 1.76 | 0.88 | 34 | 68 |
| 75 | 1.32 | 0.66 | 46 | 91 |
| 100 | 1 | 0.5 | 60 | 120 |

Maximum mana equals Intelligence. See [Stats](/stats).

## Meditating
Using the skill tries to enter a meditative trance. It can't be used:
- With anything in hand except a spellbook, a runebook, a shepherd's crook, or a light: *Your hands must be free to cast spells or meditate.*
- At full mana: *You are at peace.*
- Below `10%` of maximum hit points: *The mind is strong but the body is weak.*

The chance to succeed is `50 + 2 * (Meditation - Missing Mana)` percent, so the emptier the mana pool, the harder it is to focus.

| Missing Mana | Chance at 50 Meditation (%) | Chance at 75 Meditation (%) | Chance at 100 Meditation (%) |
|:-|:-:|:-:|:-:|
| 25 | 100 | 100 | 100 |
| 50 | 50 | 100 | 100 |
| 75 | 0 | 50 | 100 |
| 100 | 0 | 0 | 50 |

On success, the character sees *You enter a meditative trance.* A failure shows *You cannot focus your concentration.* Either way, no skill can be used for `10` seconds.

The trance halves the delay between mana points. It ends when mana is full, with *You are at peace.*, or as soon as the character moves, attacks, casts a spell, uses a skill or item, picks something up, or takes damage, with *You stop meditating.*

## Armor
Most armor slows mana regeneration, in a trance or not. The armor penalty is added to the delay before the trance halves it:

`Armor Penalty = (Body Armor + Shield Armor) / 4` seconds

Body armor is each piece's armor rating times its body slot's share, the same shares used for an armor hit: neck `7%`, hands `7%`, arms `15%`, head `14%`, legs `22%`, and chest `35%`. A shield counts its full armor rating. Leather armor adds nothing, and studded armor adds half. Exceptional quality and worn durability don't change the penalty, but a wooden shield's armor from [Carpentry](/carpentry) does.

With `100` Intelligence and `100` Meditation:

| Equipment | Delay (s) | Delay in Trance (s) |
|:-|:-:|:-:|
| No armor, or leather | 1 | 0.5 |
| Plate chest only | 4.5 | 2.25 |
| Heater shield only | 6.75 | 3.38 |
| Full plate | 7 | 5.5 |

## Spells
- Reactive Armor's maximum absorb is `(Magery + Meditation + Inscription) / 3`, up to `75`.
- Protection's chance to keep a spell from being disrupted is `(Evaluating Intelligence + Meditation + Inscription) / 4` percent, up to `75%`.

## Manual Training

## Macro Training