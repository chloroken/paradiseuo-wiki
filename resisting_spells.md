---
title: Resisting Spells
description: 
published: true
date: 2026-11-19T00:50:57.725Z
tags: 
editor: markdown
dateCreated: 2026-11-12T08:34:37.098Z
---

# Resisting Spells
Resisting Spells gives a chance to shrug off part of a hostile spell. A resisted spell does three quarters of its damage, or lasts three quarters of its duration.

## Resistable Spells
- Mind Blast
- Paralyze
- Magic Arrow
- Lightning
- Mana Drain
- Harm
- Chain Lightning
- Flame Strike
- Mana Vampire
- Meteor Swarm
- Energy Bolt
- Explosion
- Fireball
- Poison

## Resist Chance
The chance to resist a spell depends on the defender's Resisting Spells, the caster's Magery, and the spell's circle:

`Resist Chance = max(Resisting Spells / 5, Resisting Spells - ((Caster's Magery - 20) / 5 + Circle * 5)) / 2` percent

Higher-circle spells and stronger casters are harder to resist, but the chance never drops below `Resisting Spells / 10` percent.

Against a caster with `100` Magery:

| Resisting Spells | 1st Circle (%) | 4th Circle (%) | 6th Circle (%) | 8th Circle (%) |
|:-|:-:|:-:|:-:|:-:|
| 50 | 14.5 | 7 | 5 | 5 |
| 80 | 29.5 | 22 | 17 | 12 |
| 100 | 39.5 | 32 | 27 | 22 |

## Skill Gain
Resisting Spells can only gain from a spell if the defender's skill is below that circle's limit:

| Circle | Gains Below |
|:-|:-:|
| 1st | 35 |
| 2nd | 45 |
| 3rd | 55 |
| 4th | 65 |
| 5th | 75 |
| 6th | 85 |
| 7th | 120 |
| 8th | 130 |

Past `85` skill, only 7th and 8th circle spells, such as Flame Strike, Chain Lightning, and Meteor Swarm, train Resisting Spells.

## Manual Training

## Macro Training
