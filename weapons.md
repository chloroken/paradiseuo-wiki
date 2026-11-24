---
title: Weapons
description: Every weapon type, its skill, its weapon effect, and magic weapons
published: true
date: 2026-11-23T06:45:25.343Z
tags: 
editor: markdown
dateCreated: 2026-11-18T23:29:24.473Z
---

# Weapons
Each type of weapon is trained with its own skill, and most types have an effect of their own, from critical strikes to poison. Hit chance, swing speed, and damage work the same way for every weapon. See [Combat](/combat).

Damage per second is the standard way to compare weapons against monsters. See [Damage Per Second](/dps).

## Weapon Types
| Type | Skill | Weapons | Effect | Scaling Skill |
|:-|:-:|:-:|:-:|:-:|
| Swords | [Swordsmanship](/swordsmanship) | Broadsword, cutlass, katana,<br>longsword, scimitar, viking sword | [Critical strikes](#critical-strikes) | |
| Krysses | [Fencing](/fencing) | Kryss | [Poison](#poison) | |
| Axes (1H) | Swordsmanship | Pickaxe | None | [Mining](/mining) |
| Axes (2H) | Swordsmanship | Axe, battle axe, double axe, executioner's axe,<br>hatchet, large battle axe, two-handed axe | [Concussion Blow](#concussion-blow) | [Lumberjacking](/lumberjacking) |
| War Axe | [Mace Fighting](/mace_fighting) | War axe | None | |
| Polearms | Swordsmanship | Bardiche, halberd | Concussion Blow | |
| Maces (1H) | Mace Fighting | Club, hammer pick, mace, maul, war mace | [Sapping vigor](#sapping-vigor) | [Blacksmithing](/blacksmithing) |
| Maces (2H) | Mace Fighting | War hammer | [Crushing Blow](#crushing-blow) | |
| Staves | Mace Fighting | Black staff, gnarled staff, quarter staff | Crushing Blow | [Carpentry](/carpentry) |
| Shepherd's Crook | Mace Fighting | Shepherd's crook | [Shillelagh](#shillelagh) | [Herding](/herding) |
| Daggers | Fencing | Dagger | Poison | |
| Spears (1H) | Fencing | War fork | Poison | |
| Spears (2H) | Fencing | Pitchfork, short spear, spear | [Paralyzing Blow](#paralyzing-blow), poison | |
| Knives | Swordsmanship | Butcher knife, cleaver, skinning knife | Poison | |
| Bows | [Archery](/archery) | Bow, crossbow, heavy crossbow | Volley (crossbow),<br>poisoned ammunition | |
| Fists | Wrestling | Bare hands | [Stun](#wrestling-moves) | |

Crossbow volleys and poisoned ammunition are covered on the Archery page.

## Scaling Skills
Some gathering and crafting skills make their own weapons hit harder. Each bonus grows evenly up to two thirds of its total at `99.9`, and the last third comes at grandmaster. It's added to the Strength and [Anatomy](/anatomy) bonuses, so it stacks with them. See [Combat: Damage](/combat#damage).

| Scaling Skill | Weapons | Bonus at 50 (%) | Bonus at 100 (%) |
|:-|:-:|:-:|:-:|
| Lumberjacking | Axes, except the pickaxe | 10 | 30 |
| Blacksmithing | One-handed maces | 13.3 | 40 |
| Carpentry | Black, gnarled, and quarter staves | 5 | 15 |
| Mining | Pickaxe | 33.3 | 100 |

- Only players get these bonuses.
- Herding scales the shepherd's crook's [shillelagh](#shillelagh) instead of its damage.
- The war axe gets no bonus from any skill.
- Hits with axes, except the pickaxe, can train Lumberjacking. Hits never train Blacksmithing, Carpentry, Herding, or Mining.
- Carpentry also strengthens the wooden shield. See [Parrying: Shields](/parrying#shields).

## Weapon Effects
Most weapon types have a weapon effect, which can trigger when a hit lands. Weapon effects are for players only. Monsters, hirelings, and other NPCs never trigger them, even with the same weapons. Some effects also only work against monsters, as noted in their sections.

Concussion Blow, Crushing Blow, and Paralyzing Blow are triggered by Anatomy. Every hit with the right weapon has an `Anatomy / 400` chance to land one, which is `25%` at `100` Anatomy, and a character without Anatomy never lands one. The other effects have their own triggers, described in their sections.

### Critical Strikes
Swords can land a critical strike, which doubles the hit's damage before armor, including a magic weapon's damage bonus. Each sword has its own chance, scaled by Swordsmanship, so `50` Swordsmanship gives half the chance shown below. Slower swords strike critically more often, so every sword does about the same damage over time, while the slowest hit in the biggest bursts.

| Sword | Critical Strike Chance (%)<br>at 100 Swordsmanship |
|:-|:-:|
| Katana | 12 |
| Broadsword | 10 |
| Scimitar | 15 |
| Cutlass | 17 |
| Longsword | 26 |
| Viking sword | 40 |

Only swords land critical strikes, not axes, polearms, or knives. The attacker sees *You land a critical strike!* in their journal.

### Sapping Vigor
One-handed maces sap a monster's vigor. Each hit saps vigor equal to the damage dealt, and the monster's melee attacks hit as if its Strength were that much lower, down to half its normal Strength. Its health isn't affected. The sap wears off `30` seconds after the last one-handed mace hit from anyone.

The attacker sees *\*saps vigor\** over their head when a sap starts, and everyone nearby sees *\*looks drained of vigor\** when the monster is fully drained. Vigor can only be sapped from monsters. The war axe trains Mace Fighting, but has no effect on hit.

### Concussion Blow
Two-handed axes and polearms can land a Concussion Blow, which halves the target's Intelligence and lowers its maximum mana for `30` seconds. It doesn't stack.

Everyone nearby sees *\*looks concussed\** over the target.

### Crushing Blow
Two-handed maces and staves can land a Crushing Blow, which makes the target attack at half speed for `10` seconds. Another Crushing Blow restarts the time instead of stacking. The shepherd's crook is the exception and never lands one.

Crushing Blow only works against monsters. Everyone nearby sees *\*looks dazed\** over the target.

### Paralyzing Blow
Spears, short spears, and pitchforks can land a Paralyzing Blow, which freezes the target in place for `2` seconds.

Everyone nearby sees *\*looks stuck\** over the target.

### Shillelagh
In the hands of a herder, a shepherd's crook becomes a shillelagh. The first crook hit that lands after a `9` second cooldown is a bonk, which multiplies the crook's damage roll by an amount set by Herding. Everyone nearby sees *\*bonk\** over the target. When the cooldown ends, the attacker sees *Your crook hums.* in their journal.

| Herding | Bonk Damage |
|:-|:-:|
| 0 | No bonk |
| 0.1 – 9.9 | 1× |
| 10 – 19.9 | 2× |
| 20 – 29.9 | 3× |
| 30 – 39.9 | 4× |
| 40 – 49.9 | 5× |
| 50 – 59.9 | 6× |
| 60 – 69.9 | 7× |
| 70 – 79.9 | 8× |
| 80 – 89.9 | 9× |
| 90 – 100 | 10× |

- At `100` Herding, a bonk never misses.
- Below `100`, a bonk can miss. A miss shows nothing and doesn't use the bonk, so the next hit that lands bonks instead.
- The multiplier applies to the crook's damage roll, before Tactics, Strength, and Anatomy. A magic crook's damage bonus is added once and not multiplied, unlike with a critical strike.
- Otherwise a bonk is a normal hit. Armor and shields reduce it, and it's halved against players like all melee between players.
- The cooldown belongs to the player, so switching crooks doesn't reset it.
- Herding adds no damage to the crook's other hits, and the crook never lands a Crushing Blow.

### Wrestling Moves
Fighting with empty hands allows one move, Stun. It needs no button: when a punch hits and the move is off cooldown, it's attempted automatically.

- Stun freezes the target in place for `4` seconds. It works against any target, armed or not.
- It needs `80` Wrestling and `80` Anatomy, and succeeds `(Wrestling + Anatomy) / 400` of the time.
- After any attempt, it can't be used again for `10` seconds.

See [Wrestling](/wrestling) for fist damage and unarmed defense.

## Poison
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
A silver weapon does double damage against the undead. Silver is the only slayer found on weapons, and any magic weapon has a `1%` chance to be silver, on top of its other properties. Silver weapons have a silvery hue override.