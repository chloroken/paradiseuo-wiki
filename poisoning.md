---
title: Poisoning
description: 
published: true
date: 2026-11-20T04:08:35.608Z
tags: 
editor: markdown
dateCreated: 2026-11-20T00:56:57.736Z
---

# Poisoning
Poisoning is the skill of coating fencing weapons, arrows, bolts, and food with poison made with [Alchemy](/alchemy). A poisoned target takes damage every few seconds until the poison is cured or wears off. It is a dangerous skill to dabble in because any character, except grandmaster poisoners, can accidentally poison themselves in combat. See [Curing Poison](/healing#curing-poison).

## Applying Poison
Use the skill, target a poison potion, then target what to poison. After `2` seconds, a skill check decides whether it works. The skill can be used again after `10` seconds. A failure with less than `80` Poisoning has a `5%` chance to poison the character instead.

Each success lowers Karma by `20 + Karma / 100`, but never raises it: `120` at `10,000` Karma, `20` at `0`, and nothing at `-2,000` or below.

These can be poisoned:
- Fencing weapons: daggers, krysses, short spears, spears, war forks, and pitchforks
- Arrows and bolts in the backpack
- Food

Swords, knives, axes, and other weapons can't be poisoned.

| Potion | Minimum Skill | Maximum Skill | Doses |
|:-|:-:|:-:|:-:|
| Lesser poison | 0 | 60 | 18 |
| Regular poison | 30 | 70 | 16 |
| Greater poison | 60 | 100 | 14 |
| Deadly poison | 80 | 100 | 12 |

The chance to succeed rises evenly from the minimum skill, and never fails from the maximum. A potion gives `18 - 2 * Poison Level` doses. A weapon uses one dose per hit. On a stack of arrows or bolts, up to that many are coated, and the rest stay clean.

## Poisoned Weapons
A poisoned weapon uses a dose on every swing or shot.

Single-clicking a poisoned weapon, arrow, or bolt only shows that it's poisoned. A character whose Poisoning is high enough to apply that poison also sees its strength.

Arrows and bolts recovered after a shot are always clean. Poisoned ammunition only stacks with ammunition carrying the same poison, and can't go on a commodity deed. The strongest-poisoned ammunition is always used first if multiple kinds are present.

## Poison Chance
Each swing or shot that hits with a poisoned weapon or ammunition has a chance to poison the target based on Poisoning level. The chance is either `50%` or `Poisoning level * 1%`, whichever is higher. A grandmaster Poisoner that successfully hits an attack has a `100%` chance to poison.

## Self-Poisoning
Anyone can use poisoned weapons and ammunition, but every swing or shot with poison, hit or miss, risks poisoning the user with the same poison, with the message *You nick yourself and become poisoned!* The risk falls evenly from `50%` at `0` Poisoning to `5%` at `50`, then evenly to `0%` at `100`.

| Poisoning | Chance to Self-Poison (%) |
|:-|:-:|
| 0 | 50 |
| 25 | 27.5 |
| 50 | 5 |
| 75 | 2.5 |
| 100 | 0 |

The risk uses base skill, so items and spells that raise Poisoning don't count.

## Poison Strength
Each poison deals damage `10` times, then wears off, unless it's cured first. Each tick deals `1` plus a share of the target's current hit points, within a minimum and maximum. About half of the ticks repeat the previous tick's damage instead.

| Poison | Share of Current Hit Points (%) | Damage per Tick | Time Between Ticks (s) |
|:-|:-:|:-:|:-:|
| Lesser | 2.5 | 4 – 26 | 3 |
| Regular | 3.125 | 5 – 26 | 3 |
| Greater | 6.25 | 6 – 26 | 3 |
| Deadly | 12.5 | 7 – 26 | 4 |
| Lethal | 25 | 9 – 26 | 5 |

Players can't make Lethal poison. Only monsters use it.

## Manual Training

## Macro Training