---
title: Combat
description: Hit chance, swing speed, and damage
published: true
date: 2026-11-28T08:30:00.000Z
tags: 
editor: markdown
dateCreated: 2026-11-26T18:40:29.000Z
---

# Combat
This page covers how [often attacks land](#hit-chance), how [fast they come](#swing-speed), and how much [damage they do](#damage).

Characters who fight without magic also gain accuracy, toughness, and regeneration through [Valor](/valor).

## Gear and Skills
- [Weapons](/weapons): every weapon type, its skill, and its scaling skill.
- [Weapon Effects](/weapon_effects): critical strikes, blows, the shillelagh, and other effects on hit.
- [Magic Weapons](/magic_weapons): damage, accuracy, durability, and silver properties.
- [Armor](/armor): how armor and shields reduce damage.
- [Archery](/archery): bows and crossbows, and ammunition.
- [Ambush](/ambush): extra damage when attacking from Hiding and Stealth.
- [Wrestling](/wrestling): bare-handed moves and unarmed defense.
- [Parrying](/parrying): blocking with shields, and Valor's toughness.
- [Tactics](/tactics): more damage with every weapon, and Valor's accuracy.
- [Anatomy](/anatomy): more damage, wrestling stuns, polearm Concussion Blows, better bandages, and Valor's regeneration.
- [Arms Lore](/arms_lore): weapon effects, such as critical strikes and Crushing Blow.
- [Healing](/healing): bandages that heal, cure poison, and resurrect.
- [Poisoning](/poisoning): coating weapons and ammunition, and how [poison](/poison) works once it lands.
- [Hiding](/hiding) and [Stealth](/stealth): disappearing and moving unseen before an ambush.
- [Tracking](/tracking): finding targets, and accuracy with ranged weapons.
- [Monsters](/monsters): what there is to fight.

## Swing Speed
The delay between attacks depends on the weapon's speed and the attacker's current stamina:

`15000 / ((Stamina + 100) * Weapon Speed)` seconds

Every weapon has a hidden speed value, with lighter weapons faster than heavy ones. Current stamina is used, not maximum stamina, so a tired fighter swings more slowly. At `50` stamina, each swing takes a third longer than at `100`. This is why fighters want high [Dexterity](/stats#dexterity).

## Hit Chance
Each attack compares the attacker's weapon skill to the defender's:

`(Attacker's Weapon Skill + 50) / ((Defender's Weapon Skill + 50) * 2)`

The defender uses the skill of whatever weapon they're holding, so a fencer defends with Fencing and an archer with Archery. An unarmed player defends with [Wrestling](/wrestling#unarmed-defense) alone.

| Attacker Skill | Defender Skill | Hit Chance (%) |
|:-|:-:|:-:|
| 100 | 0 | 100 |
| 100 | 50 | 75 |
| 100 | 80 | 58 |
| 100 | 100 | 50 |
| 50 | 100 | 33 |

Every attack, hit or miss, has a chance to raise the attacker's weapon skill.

Two things can raise hit chance beyond skill:
- Valor adds to the attacker's weapon skill for this roll.
- Ambushers gain accuracy for every [stealthed step](/ambush#stealth) before the attack, until it can't miss.

## Damage
Every weapon rolls its base damage, which is then changed in two steps.

First, Tactics changes the damage by `(Tactics - 50)%`, from `-50%` at `0` to `+50%` at `100`. A character with no Tactics does half damage.

Second, these bonuses are added together, then applied to the result:

| Source | Bonus | At 100 (%) |
|:-|:-:|:-:|
| Strength | 1% per 5 Strength | 20 |
| Anatomy | 1% per 5 Anatomy, plus 10% at grandmaster | 30 |
| [Scaling skills](/weapons#scaling-skills) | Lumberjacking for axes, Carpentry for staves, Mining for the pickaxe | 15 – 100 |
| [Weapon quality](/crafting#exceptional-items) | +20% exceptional | |

A fighter with `100` in Tactics, Strength, and Anatomy does `1.5 * 1.5 = 2.25` times the weapon's base damage. With an exceptional weapon, that rises to `1.5 * 1.7 = 2.55` times, and with an exceptional axe and `100` Lumberjacking, to `1.5 * 2.0 = 3` times.

Magic and exceptional damage are [flat modifiers](/magic_weapons#modifiers), so critical strikes, ambushes, and bonks multiply only the weapon's own roll.

A worn-out weapon does less damage, down to half when it's about to break.

Melee damage between players is halved, and so is melee damage from a player's [follower](/follower) to another player. Every other hit between players and monsters does full damage, so monsters hit players twice as hard as on most ServUO shards.

A [demiboss](/demibosses) does [double damage](/follower#followers-in-combat) to every follower, except with breath, poison, and Fire Field.

The damage of each hit shows as a number over the target. The attacker and the target see it, as do the owners of any followers involved.

Valor, shields, [armor](/armor#how-armor-works), and Arch Protection then reduce the damage before it reaches the target.

## Being Hit
- Any damage, however small, makes a [bandage slip](/healing#slips).
- Frozen characters can't move or begin casting a spell, but can still attack anything in reach. Wrestling stuns and Paralyzing Blow freeze their target, and the freeze lasts its full time, even through damage.
- Paralyzed characters have the same limits, but taking damage breaks the paralysis. The Paralyze spell and paralyze fields paralyze their target.