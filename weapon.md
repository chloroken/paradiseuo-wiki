---
title: Weapon
description: 
published: true
date: 2026-11-18T23:34:48.427Z
tags: 
editor: markdown
dateCreated: 2026-11-18T23:29:24.473Z
---

# Weapon
Weapons are split into types, and each type is trained with its own skill. Some types have special attacks or other effects on hit.

## Weapon Types
| Type | Skill | Examples |
|:-|:-:|:-:|
| Swords | [Swordsmanship](/swordsmanship) | Longswords, katanas, scimitars |
| Kryss and Lances | [Fencing](/fencing) | Kryss, lances |
| Axes | Swordsmanship | Battle axes, double axes, executioner's axes |
| War Axe | [Mace Fighting](/mace_fighting) | War axe |
| Polearms | Swordsmanship | Halberds, bardiches |
| Maces | Mace Fighting | Maces, war hammers, mauls |
| Staves | Mace Fighting | Quarter staves, gnarled staves, black staves |
| Daggers | Fencing | Daggers |
| Spears | Fencing | Spears, short spears, pikes |
| Knives | Swordsmanship | Cleavers, butcher knives, skinning knives |
| Bows | [Archery](/archery) | Bows, crossbows, heavy crossbows |
| Fists | [Wrestling](/wrestling) | Bare hands |

## Special Attacks
Two-handed axes, polearms, maces, and spears each have a special attack. Every hit has an `Anatomy / 400` chance to trigger it, which is `25%` at `100` [Anatomy](/anatomy).

| Special | Weapons | Effect |
|:-|:-:|:-:|
| Concussion Blow | Two-handed axes and polearms | Halves the target's Intelligence for 30 seconds. Doesn't stack. |
| Crushing Blow | Two-handed maces | 1.5× base damage |
| Paralyzing Blow | Two-handed spears | Freezes the target in place for 2 seconds |

Concussion Blow and Crushing Blow can only be delivered by players and human NPCs. Concussion Blow lowers maximum mana, so it is especially strong against spellcasters.

A frozen target can't move, but it can still attack anything in reach. Freezing is most useful against a target that is fleeing or chasing.

## Wrestling Moves
Fighting with bare hands allows two moves, readied with the client's stun or disarm button. The move is attempted on the next hit.

| Move | Requirements | Effect |
|:-|:-:|:-:|
| Stun | 80 Wrestling, 80 Anatomy, 15 stamina | Freezes the target in place for 4 seconds |
| Disarm | 80 Wrestling, 80 Arms Lore, 15 stamina | Knocks the target's weapon into their backpack |

- Each attempt costs `15` stamina, even if it fails.
- The chance to succeed is `(Wrestling + Anatomy) / 400` for Stun, and `(Wrestling + Arms Lore) / 400` for Disarm: `40%` at 80 in both skills, and `50%` at 100.
- Disarm only works on players and human NPCs.
- After a successful move, another can't be used for `10` seconds.

## Other Effects on Hit
- Maces and staves drain `3` to `5` of the target's stamina with every hit.
- Axes gain bonus damage from [Lumberjacking](/lumberjacking), up to `20%` at grandmaster.
- Swords, knives, daggers, and spears coated with [Poisoning](/poisoning) have a `50%` chance per hit to poison the target, using one charge each hit.
- Arrows and bolts that hit a monster or animal have a `40%` chance to land in its backpack, where they can be looted back. Missed shots have a `40%` chance to drop on the ground.

## Unarmed Defense
When fighting with bare hands, a character defends with whichever is higher: their Wrestling, or `(Anatomy + Evaluating Intelligence + 20) / 2`, up to `120`. This means a mage with `100` [Evaluating Intelligence](/evaluating_intelligence) defends as if they had `60` Wrestling, even with none.