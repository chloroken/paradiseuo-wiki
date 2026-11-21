---
title: Weapon
description: 
published: true
date: 2026-11-21T06:15:28.888Z
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

Everyone nearby sees a special land: the target shows *\*looks concussed\**, *\*looks dazed\**, or *\*looks stuck\**. A player hit by Concussion Blow or Paralyzing Blow also gets a message in their journal.

## Other Effects on Hit
### Critical Strikes
Swords can land a critical strike, which doubles the hit's damage before armor. Each sword has its own chance, scaled by Swordsmanship, so `50` Swordsmanship gives half the chance shown below. Slower swords strike critically more often, so every sword does about the same damage over time, while the slowest hit in the biggest bursts. Only players can land critical strikes, and only with swords, not axes, polearms, or knives. The attacker sees *\*critical strike\** over their head.

| Sword | Critical Strike Chance at 100 Swordsmanship (%) |
|:-|:-:|
| Katana | 12 |
| Broadsword | 10 |
| Cutlass | 10 |
| Scimitar | 15 |
| Longsword | 26 |
| Viking sword | 40 |

### Sapping Vigor
One-handed maces sap a monster's vigor. Each hit saps vigor equal to the damage dealt, and the monster's melee attacks hit as if its Strength were that much lower, down to half its normal Strength. Its health isn't affected. The sap wears off `30` seconds after the last one-handed mace hit from anyone.

The attacker sees *\*saps vigor\** over their head when a sap starts, and everyone nearby sees *\*looks drained of vigor\** when the monster is fully drained. Only players can sap vigor, and only from monsters. The war axe trains Mace Fighting, but has no effect on hit.

### Poison
Fencing weapons and knives can be coated with poison, which can poison the target on a hit, but risks poisoning a wielder without Poisoning. See [Poisoning](/poisoning).

## Magic Weapons
Weapons found as loot can be magic. A magic weapon can have a damage, accuracy, and durability property, each in five strengths, and some weapons are slayers instead.

### Damage
| Property | Base Damage Bonus |
|:-|:-:|
| Ruin | +1 |
| Might | +3 |
| Force | +5 |
| Power | +7 |
| Vanquishing | +9 |

The bonus is added to the weapon's base damage before Tactics, Strength, and Anatomy, so a fighter with `100` in all three gets `2.25` times the bonus. Fast weapons gain the most, since they hit more often. A crossbow only adds the bonus to the first bolt of each volley.

### Accuracy
| Property | Weapon Skill Bonus |
|:-|:-:|
| Accurate | +5 |
| Surpassingly accurate | +10 |
| Eminently accurate | +15 |
| Exceedingly accurate | +20 |
| Supremely accurate | +25 |

The bonus raises the weapon's skill while it's held, which improves both hit chance and defense. See [Hit Chance](/combat#hit-chance).

### Durability
| Property | Maximum Durability Bonus (%) |
|:-|:-:|
| Durable | 20 |
| Substantial | 50 |
| Massive | 70 |
| Fortified | 100 |
| Indestructible | 120 |

### Silver
A silver weapon does double damage against the undead. Silver is the only slayer found on weapons, and any magic weapon has a `5%` chance to be silver, on top of its other properties. Silver weapons have a silvery color.