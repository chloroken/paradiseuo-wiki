---
title: Weapons
description: 
published: true
date: 2026-11-21T17:32:48.483Z
tags: 
editor: markdown
dateCreated: 2026-11-18T23:29:24.473Z
---

# Weapons
Each type of weapon is trained with its own skill, and most types have an effect of their own, from critical strikes to poison. Hit chance, swing speed, and damage work the same way for every weapon. See [Combat](/combat).

## Weapon Types
| Type | Skill | Weapons | Effect |
|:-|:-:|:-:|:-:|
| Swords | [Swordsmanship](/swordsmanship) | Broadsword, cutlass, katana, longsword, scimitar, viking sword | [Critical strikes](#critical-strikes) |
| Krysses | [Fencing](/fencing) | Kryss | [Poison](#poison) |
| Axes (one-handed) | Swordsmanship | Pickaxe | None |
| Axes (two-handed) | Swordsmanship | Axe, battle axe, double axe, executioner's axe,<br>hatchet, large battle axe, two-handed axe | [Concussion Blow](#concussion-blow) |
| War Axe | [Mace Fighting](/mace_fighting) | War axe | None |
| Polearms | Swordsmanship | Bardiche, halberd | Concussion Blow |
| Maces (one-handed) | Mace Fighting | Club, hammer pick, mace, maul, war mace | [Sapping vigor](#sapping-vigor) |
| Maces (two-handed) | Mace Fighting | War hammer | [Crushing Blow](#crushing-blow) |
| Staves | Mace Fighting | Black staff, gnarled staff, quarter staff, shepherd's crook | Crushing Blow |
| Daggers | Fencing | Dagger | Poison |
| Spears (one-handed) | Fencing | War fork | Poison |
| Spears (two-handed) | Fencing | Pitchfork, short spear, spear | [Paralyzing Blow](#paralyzing-blow), poison |
| Knives | Swordsmanship | Butcher knife, cleaver, skinning knife | Poison |
| Bows | [Archery](/archery) | Bow, crossbow, heavy crossbow | Crossbow volley, poisoned ammunition |
| Fists | Wrestling | Bare hands | [Disarm and Stun](#wrestling-moves) |

Crossbow volleys and poisoned ammunition are covered on the Archery page.

## Weapon Effects
Most weapon types have an effect on hit. Only players can trigger most of them, and several only work against monsters.

Two-handed axes, polearms, maces, and spears each have a special attack, and staves count as two-handed maces. Every hit has an `Anatomy / 400` chance to trigger it, which is `25%` at `100` [Anatomy](/anatomy).

### Critical Strikes
Swords can land a critical strike, which doubles the hit's damage before armor. Each sword has its own chance, scaled by Swordsmanship, so `50` Swordsmanship gives half the chance shown below. Slower swords strike critically more often, so every sword does about the same damage over time, while the slowest hit in the biggest bursts.

| Sword | Critical Strike Chance (%)<br>at 100 Swordsmanship |
|:-|:-:|
| Katana | 12 |
| Broadsword | 10 |
| Cutlass | 10 |
| Scimitar | 15 |
| Longsword | 26 |
| Viking sword | 40 |

Only players can land critical strikes, and only with swords, not axes, polearms, or knives. The attacker sees *You land a critical strike!* in their journal.

### Sapping Vigor
One-handed maces sap a monster's vigor. Each hit saps vigor equal to the damage dealt, and the monster's melee attacks hit as if its Strength were that much lower, down to half its normal Strength. Its health isn't affected. The sap wears off `30` seconds after the last one-handed mace hit from anyone.

The attacker sees *\*saps vigor\** over their head when a sap starts, and everyone nearby sees *\*looks drained of vigor\** when the monster is fully drained. Only players can sap vigor, and only from monsters. The war axe trains Mace Fighting, but has no effect on hit.

### Concussion Blow
Two-handed axes and polearms can land a Concussion Blow, which halves the target's Intelligence and lowers its maximum mana for `30` seconds. It doesn't stack.

Only players and human NPCs can deliver a Concussion Blow. Everyone nearby sees *looks concussed* over the target.

### Crushing Blow
Two-handed maces and staves can land a Crushing Blow, which makes the target attack at half speed for `10` seconds. Another Crushing Blow restarts the time instead of stacking.

Only players can deliver a Crushing Blow, and only against monsters. Everyone nearby sees *looks dazed* over the target.

### Paralyzing Blow
Spears, short spears, and pitchforks can land a Paralyzing Blow, which freezes the target in place for `2` seconds.

Everyone nearby sees *looks stuck* over the target.

### Wrestling Moves
Fighting with empty hands allows two moves, Disarm and Stun. Neither needs a button: when a punch hits and the moves are off cooldown, the right one is attempted automatically.

- Disarm is used against armed players and human NPCs, and knocks the target's weapon into their backpack. It needs `80` Wrestling and `80` Arms Lore, and succeeds `(Wrestling + Arms Lore) / 400` of the time.
- Stun is used against everything else, and freezes the target in place for `4` seconds. It needs `80` Wrestling and `80` Anatomy, and succeeds `(Wrestling + Anatomy) / 400` of the time.
- Against an armed human, a wrestler without `80` Arms Lore stuns instead.
- After any attempt, neither move can be used again for `10` seconds.

See [Wrestling](/wrestling) for fist damage and unarmed defense.

### Poison
Fencing weapons and knives can be coated with poison, which can poison the target on a hit, but risks poisoning a wielder without Poisoning. See [Poisoning](/poisoning).

## Magic Weapons
Weapons found as loot can be magic. A magic weapon can have a damage, accuracy, and durability property, each in five strengths, and can also be [silver](#silver).

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
A silver weapon does double damage against the undead. Silver is the only slayer found on weapons, and any magic weapon has a `1%` chance to be silver, on top of its other properties. Silver weapons have a silvery color.

A liche's ring turns any weapon silver, but kills its user. See [Lich King: Liche's Ring](/lich_king#liches-ring).