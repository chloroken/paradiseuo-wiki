---
title: Evaluating Intelligence
description: More spell damage, judging a target's mind, unarmed defense, and Protection
published: true
date: 2026-11-25T01:58:26.522Z
tags: 
editor: markdown
dateCreated: 2026-11-24T08:17:34.020Z
---

# Evaluating Intelligence
Evaluating Intelligence is the skill of judging a mind. Its main use is making [Magery](/magery)'s damage spells hit harder. It also lets a mage defend with empty hands, and strengthens the [Protection](/protection) spell.

## Spell Damage
Damage spells compare the caster's Evaluating Intelligence to the target's [Resisting Spells](/resisting_spells):
- When Evaluating Intelligence is higher, damage rises by `(Evaluating Intelligence - Resisting Spells) / 5` percent, up to `20%`.
- When it's lower, damage falls by `(Resisting Spells - Evaluating Intelligence) / 2` percent, down to `-50%`.

| Evaluating Intelligence | Damage Against<br>0 Resisting Spells (%) | Damage Against<br>50 Resisting Spells (%) | Damage Against<br>100 Resisting Spells (%) |
|:-|:-:|:-:|:-:|
| 0 | 100 | 75 | 50 |
| 50 | 110 | 100 | 75 |
| 100 | 120 | 110 | 100 |

Falling behind costs more than getting ahead gains, so a caster without Evaluating Intelligence does half damage to a target with `100` Resisting Spells.

The caster's Magery then adds `(Magery - 100) / 4` percent, from `-25%` at `0` to nothing at `100`. Against monsters and animals, the result is doubled. Against players and creatures with a human body, it isn't. A resisted spell then does three quarters of the damage.

These spells use Evaluating Intelligence:
- Magic Arrow
- Harm
- Fireball
- Lightning
- Mind Blast
- Energy Bolt
- Explosion
- Chain Lightning
- Flame Strike
- Meteor Swarm

Other spells, including Earthquake, Poison, and the field spells, don't use it. Spell durations and the strength of curses and buffs come from Magery. See [Spells](/spells).

## Examining
Using the skill and targeting a person or creature within `8` tiles describes how intelligent it looks. From `76` Evaluating Intelligence, it also describes how much of its mana the target has left. The description can be off by up to `20 - Evaluating Intelligence / 5` points of Intelligence, and the same in percent for mana, so it's exact at `100`.

An attempt succeeds `Evaluating Intelligence / 120` of the time, so `83%` of the time at `100`. A failed attempt gives no information.

## Unarmed Defense
A character with empty hands defends with `(Anatomy + Evaluating Intelligence + 20) / 2` when that's higher than their Wrestling, up to `120`. With `100` Evaluating Intelligence alone, that's `60`, and with `100` [Anatomy](/anatomy) as well, it's `110`. See [Wrestling: Unarmed Defense](/wrestling#unarmed-defense).

## Protection
Evaluating Intelligence raises the Protection spell's chance to keep a spell from being disrupted, along with [Meditation](/meditation) and [Inscription](/inscription). The chance is `(Evaluating Intelligence + Meditation + Inscription) / 4` percent, up to `75%`.

## Manual Training
Use the Evaluating Intelligence skill on others. Targeting player characters gives the best gains. Can use the same target repetitively with no penalty.

## Macro Training
Double click a player to designate them as `Last Target` before running the macro.
- `Use Skill: Evaluating Intelligence`
- `Wait For Target`
- `Last Target`
- `Delay 1000ms`

It takes 30-60 minutes to grandmaster.