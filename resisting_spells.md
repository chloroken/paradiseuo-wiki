---
title: Resisting Spells
description: 
published: true
date: 2026-11-18T22:49:46.355Z
tags: 
editor: markdown
dateCreated: 2026-11-12T08:34:37.098Z
---

# Resisting Spells
A resisted spell does three quarters of its damage, or lasts three quarters of its duration.

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
- `A = Resisting Spells / 5`
- `B = (Caster's Magery - 20) / 5 + (1 + Circle) * 5`, which ranges from `20` to `95` (8th circle)
- `X` is whichever of `A` or `B` is higher.

`X` is then divided by `2`, then by `100`, giving `0.10` to `0.475` (8th circle):
- If `X <= 0`, the spell is never resisted.
- If `X >= 1`, the spell is always resisted.

## Skill Gain
A resist check is eligible for skill gain if `X >= 0.1`.

- `C = (1 + Circle) * 10 + (1 + Circle / 6) * 25`, for example `127.5`
- If `X` (`0.1` to `0.475`) is below `C`, Resisting Spells can gain.
- The resist itself is then checked, with `X` between `0` and `1`.

## Manual Training

## Macro Training
