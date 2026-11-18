---
title: Resisting Spells
description: 
published: true
date: 2026-11-15T03:50:48.080Z
tags: 
editor: markdown
dateCreated: 2026-11-12T08:34:37.098Z
---

# Resisting Spells
A resisted spell does 3/4 damage or has 3/4 duration.

Resistable spells:
- Mind Blast
- Paralyze
- magic Arrow
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

Formula

A = `Resisting Spells / 5`
B = Caster's `(Magery - 20) / 5 + (1 + circle) * 5`
20 vs 95(circle8)
X = Return A or B, whichever is higher

X / 2
X / 100
.10 vs .475(circle8)
if X <= 0, no resist
if X >= 1, resist

Gains formula:

if >= .1, eligible

C = `(1 + circle) * 10 + (1 + circle / 6) * 25`
C = 127.5

if `.1 or .475 < C`, resist gain
then check for resist with X >= 0~1.0