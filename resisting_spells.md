---
title: Resisting Spells
description: Resist chance against hostile spells, and which spells train it
published: true
date: 2026-11-26T12:02:01.505Z
tags: 
editor: markdown
dateCreated: 2026-11-12T08:34:37.098Z
---

# Resisting Spells
Resisting Spells gives a chance to shrug off part of a hostile spell. How much a resist blocks depends on the spell. See [Resistible Spells](#resistible-spells).

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

## Resistible Spells
| Spell | Circle | When Resisted |
|:-|:-:|:-:|
| Magic Arrow | 1st | 75% damage |
| Harm | 2nd | 75% damage |
| Fireball | 3rd | 75% damage |
| Poison | 3rd | No effect |
| Lightning | 4th | 75% damage |
| Mana Drain | 4th | No effect |
| Mind Blast | 5th | 50% damage |
| Paralyze | 5th | 75% duration |
| Energy Bolt | 6th | 75% damage |
| Explosion | 6th | 75% damage |
| Chain Lightning | 7th | 50% damage |
| Flame Strike | 7th | 60% damage |
| Mana Vampire | 7th | No effect |
| Meteor Swarm | 7th | 50% damage |

Chain Lightning and Meteor Swarm split their damage evenly among every target they hit, so a single target takes the full amount.

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