---
title: Combat
description: 
published: true
date: 2026-11-19T07:58:25.523Z
tags: 
editor: markdown
dateCreated: 2026-11-19T00:05:40.279Z
---

# Combat
Combat on *Paradise* follows T2A rules, apart from the changes marked 𐠒. This page covers how often attacks land, how fast they come, how much damage they do, and the extra toughness given to characters without Magery. For weapon types and special attacks, see [Weapon](/weapon), and for Wrestling moves, see [Wrestling](/wrestling).

## Swing Speed
The delay between attacks depends on the weapon's speed and the attacker's current stamina:

`15000 / ((Stamina + 100) * Weapon Speed)` seconds

Every weapon has a hidden speed value, with lighter weapons faster than heavy ones. Current stamina is used, not maximum stamina, so a tired fighter swings more slowly. At `50` stamina, each swing takes a third longer than at `100`. This is why fighters want high [Dexterity](/stats#dexterity), and why maces and staves, which drain stamina on every hit, are dangerous to fight against.

## Hit Chance
Each attack compares the attacker's weapon skill to the defender's:

`(Attacker's Weapon Skill + 50) / ((Defender's Weapon Skill + 50) * 2)`

The defender uses the skill of whatever weapon they're holding, so a fencer defends with Fencing and an archer with Archery. An empty-handed character defends with Wrestling, or with Anatomy and Evaluating Intelligence. See [Unarmed Defense](/wrestling#unarmed-defense).

| Attacker Skill | Defender Skill | Hit Chance (%) |
|:-|:-:|:-:|
| 100 | 0 | 100 |
| 100 | 50 | 75 |
| 100 | 80 | 58 |
| 100 | 100 | 50 |
| 50 | 100 | 33 |

Every attack, hit or miss, has a chance to raise the attacker's weapon skill.

Two things can raise hit chance beyond skill:
- Antimage adds to the attacker's weapon skill for this roll. See [Antimage](#antimage).
- Stealth archers gain accuracy for every stealthed step before an ambush 𐠒, until the shot can't miss. See [Archery](/archery).

## Damage
Every weapon rolls its base damage, which is then changed in two steps.

First, [Tactics](/tactics) changes the damage by `(Tactics − 50)%`, from `−50%` at `0` to `+50%` at `100`. A character with no Tactics does half damage.

Second, these bonuses are added together, then applied to the result:

| Source | Bonus | At 100 (%) |
|:-|:-:|:-:|
| Strength | 1% per 5 Strength | 20 |
| [Anatomy](/anatomy) | 1% per 5 Anatomy, plus 10% at grandmaster | 30 |
| [Lumberjacking](/lumberjacking) | 1% per 5 Lumberjacking, axes only | 20 |
| Weapon quality | +20% exceptional, −20% low quality | |

A fighter with `100` in Tactics, Strength, and Anatomy does `1.5 * 1.5 = 2.25` times the weapon's base damage. With an exceptional weapon, that rises to `1.5 * 1.7 = 2.55` times, and with an exceptional axe and `100` Lumberjacking, to `1.5 * 1.9 = 2.85` times.

A worn-out weapon does less damage, down to half when it's about to break.

Armor then absorbs part of the damage before it reaches the target. See [Armor](/armor).

## Being Hit
- Any damage, however small, makes a bandage slip. See [Slips](/healing#slips).
- Frozen characters can't move or begin casting a spell, but can still attack anything in reach. Wrestling stuns and Paralyzing Blow freeze their target, and the freeze lasts its full time, even through damage.
- Paralyzed characters have the same limits, but taking damage breaks the paralysis. The Paralyze spell and paralyze fields paralyze their target.

## Antimage 𐠒
Characters with little or no Magery get three bonuses in combat, meant to make fighting with weapons, in melee or at range, as fun as playing a tamer, bard, or mage. Each bonus is at its full size with `0` Magery, shrinks evenly as Magery rises, and is gone at `100`. Only players get these bonuses, not monsters or pets.

- Accuracy: Tactics adds up to `30` points to the attacker's weapon skill when rolling to hit, for every kind of weapon, including bows and bare hands. The bonus is `30 * (Tactics / 100) * ((100 − Magery) / 100)` points.
- Toughness: physical damage taken is reduced by up to `20%`, after armor. This covers weapons and monsters' melee attacks, but not spells, breath, or poison.
- Regeneration: hit points regenerate up to `5` times as fast.

| Magery | Accuracy Bonus (points at 100 Tactics) | Damage Taken (%) | Regeneration Speed |
|:-|:-:|:-:|:-:|
| 0 | 30 | 80 | 5× |
| 25 | 22.5 | 85 | 4× |
| 50 | 15 | 90 | 3× |
| 75 | 7.5 | 95 | 2× |
| 100 | 0 | 100 | 1× |

With `100` Tactics, `100` weapon skill, and no Magery, a fighter hits a defender with `100` skill `60%` of the time instead of `50%`, and hits a monster with `80` Wrestling `69%` of the time instead of `58%`.

The bonuses check the character's Magery at all times, so raising or lowering Magery changes them immediately. These numbers are being tested during alpha and may change.