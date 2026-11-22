---
title: Poison
description: Poison strengths, how characters get poisoned, and how to cure it
published: true
date: 2026-11-20T04:21:01.590Z
tags: 
editor: markdown
dateCreated: 2026-11-20T04:15:46.683Z
---

# Poison
Poison damages a character or creature every few seconds until it wears off or is cured. It comes from monsters, poisoned weapons and ammunition, spells, and food.

## Strength
Poison comes in five strengths. Each one deals damage `10` times, then wears off, unless it's cured first. Each tick deals `1` plus a share of the target's current hit points, within a minimum and maximum. About half of the ticks repeat the previous tick's damage instead.

| Poison | Level | Share of Current Hit Points (%) | Damage per Tick | Time Between Ticks (s) |
|:-|:-:|:-:|:-:|:-:|
| Lesser | 0 | 2.5 | 4 – 26 | 3 |
| Regular | 1 | 3.125 | 5 – 26 | 3 |
| Greater | 2 | 6.25 | 6 – 26 | 3 |
| Deadly | 3 | 12.5 | 7 – 26 | 4 |
| Lethal | 4 | 25 | 9 – 26 | 5 |

Players can't make Lethal poison. Only monsters use it.

## Getting Poisoned
A poisoned character can only be poisoned again by a stronger poison, which replaces the current one. A poison of equal or lower strength has no effect.

[Young players](/young_player) can't be poisoned.

### Poisoned Weapons
Fencing weapons, knives, arrows, and bolts coated with [Poisoning](/poisoning) can poison their target on a hit. The chance is the attacker's Poisoning skill as a percentage, but never below `50%`. See [Poisoned Weapons](/poisoning#poisoned-weapons).

## Poisoning Spellcasters
Monsters with Magery cast Cure on themselves before anything else. Every time a poisoner poisons them again, they spend another spell curing it instead of attacking, so poison wears mages down and keeps their spells off the poisoner.

### Poison Spell
The Poison spell's strength depends on the caster's combined Magery and Poisoning. The total drops by `10` for every tile beyond `3` between the caster and the target.

| Magery + Poisoning | Poison |
|:-|:-:|
| 130 or below | Lesser |
| Above 130 | Regular |
| Above 170 | Greater |
| 200 | Greater, with a 10% chance of Deadly |

[Poison Field](/poison_field) always applies Regular poison.

### Other Sources
- Some monsters poison their targets when they hit.
- Eating poisoned food poisons the eater with the food's poison.

## Curing Poison
### Spells
[Cure](/cure) cures one target, and [Arch Cure](/arch_cure) cures everyone nearby. The chance to cure is `100 + 0.75 * Magery - 17.5 * (Level + 1)` percent, using the poison's level from the table above. Arch Cure's chance is `1%` lower.

| Poison | Cure at 50 Magery (%) | Cure at 100 Magery (%) |
|:-|:-:|:-:|
| Lesser | 100 | 100 |
| Regular | 100 | 100 |
| Greater | 85 | 100 |
| Deadly | 67 | 100 |
| Lethal | 50 | 87 |

### Potions
| Poison | Lesser Cure (%) | Cure (%) | Greater Cure (%) |
|:-|:-:|:-:|:-:|
| Lesser | 75 | 100 | 100 |
| Regular | 50 | 75 | 100 |
| Greater | 15 | 50 | 100 |
| Deadly | 0 | 15 | 75 |
| Lethal | 0 | 0 | 25 |

### Bandages
Bandaging a poisoned target always tries to cure the poison instead of healing. See [Healing: Curing Poison](/healing#curing-poison) and [Veterinary](/veterinary) for creatures.