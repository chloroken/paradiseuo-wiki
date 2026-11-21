---
title: Weapon
description: 
published: true
date: 2026-11-20T16:51:22.381Z
tags: 
editor: markdown
dateCreated: 2026-11-18T23:29:24.473Z
---

# Weapon
Each type of weapon is trained with its own skill, and some types have special attacks or other effects on hit. Hit chance, swing speed, and damage work the same way for every weapon. See [Combat](/combat).

## Weapon Types
| Type | Skill | Examples |
|:-|:-:|:-:|
| Swords | [Swordsmanship](/swordsmanship) | Longsword, katana, scimitar |
| Krysses | [Fencing](/fencing) | Kryss |
| Axes | Swordsmanship | Battle axe, double axe, executioner's axe |
| War Axe | [Mace Fighting](/mace_fighting) | War axe |
| Polearms | Swordsmanship | Halberd, bardiche |
| Maces | Mace Fighting | Mace, war hammer, maul |
| Staves | Mace Fighting | Quarter staff, gnarled staff, black staff |
| Daggers | Fencing | Dagger |
| Spears | Fencing | Spear, short spear |
| Knives | Swordsmanship | Cleaver, butcher knife, skinning knife |
| Bows | [Archery](/archery) | Bow, crossbow, heavy crossbow |
| Fists | Wrestling | Bare hands |

Fighting with bare hands has its own automatic moves and unarmed defense. See [Wrestling](/wrestling).

## Special Attacks
Two-handed axes, polearms, maces, and spears each have a special attack, and staves count as two-handed maces. Every hit has an `Anatomy / 400` chance to trigger it, which is `25%` at `100` [Anatomy](/anatomy).

| Special | Weapons | Effect |
|:-|:-:|:-:|
| Concussion Blow | Two-handed axes and polearms | Halves the target's Intelligence for 30 seconds. Doesn't stack. |
| Crushing Blow | Two-handed maces and staves | The target attacks at half speed for 10 seconds. Another Crushing Blow restarts the time instead of stacking. |
| Paralyzing Blow | Two-handed spears | Freezes the target in place for 2 seconds |

Concussion Blow can only be delivered by players and human NPCs, and also lowers the target's maximum mana. Crushing Blow can only be delivered by players, and only against monsters.

## Other Effects on Hit
### Critical Strikes
Swords can land a critical strike, which doubles the hit's damage before armor. Each sword has its own chance, scaled by Swordsmanship, so `50` Swordsmanship gives half the chance shown below. Slower swords strike critically more often, so every sword does about the same damage over time, while the slowest hit in the biggest bursts. Only players can land critical strikes, and only with swords, not axes, polearms, or knives.

| Sword | Critical Strike Chance at 100 Swordsmanship (%) |
|:-|:-:|
| Katana | 12 |
| Broadsword | 10 |
| Cutlass | 10 |
| Scimitar | 15 |
| Longsword | 26 |
| Viking sword | 40 |

### Weakening Blows
One-handed maces weaken monsters. Each hit lowers the monster's Strength by the damage dealt, down to half its normal Strength, which makes its own melee attacks weaker. The loss wears off `30` seconds after the last one-handed mace hit from anyone. Only players can weaken monsters this way, and it never affects players. The war axe trains Mace Fighting, but has no effect on hit.

### Poison
Fencing weapons and knives can be coated with poison, which can poison the target on a hit, but risks poisoning a wielder without Poisoning. See [Poisoning](/poisoning).