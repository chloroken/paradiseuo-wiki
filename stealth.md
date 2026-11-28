---
title: Stealth
description: Moving while hidden, its requirements, and its role in an ambush
published: true
date: 2026-11-28T09:45:25.880Z
tags: 
editor: markdown
dateCreated: 2026-11-19T07:34:20.704Z
---

# Stealth
Stealth is the skill of moving while hidden. A character usually has to be hidden with [Hiding](/hiding) first, but a grandmaster at both Hiding and Stealth can use Stealth to [vanish](#vanish) in the middle of a fight.

## Requirements
- At least `80` Hiding, or the attempt fails with *You are not hidden well enough*.
- Light armor. Armor totaling `26` or more armor rating makes stealth impossible, and any armor makes it harder.
- No mount. Riding while hidden reveals the character as soon as they move.

## Moving Quietly
Stealth is used like any other skill, while already hidden. Using it while visible tries to vanish instead. On success, the character can walk `1` step for every `10` points of Stealth, so `10` steps at `100` skill. Once those steps run out, the next step reveals the character, so Stealth has to be used again before then. A failed attempt reveals the character.

The chance to succeed is `(Stealth + 20 - 2 * Armor Rating)%`. Without armor, it never fails from `80` Stealth.

- Running while hidden reveals the character at once.
- After each attempt, the skill can't be used again for `10` seconds.

## Vanish
Using Stealth while visible vanishes the character: they hide at once and can start walking, even with monsters fighting them right next to them. Monsters lose sight of the character, who can simply walk away. It needs:
- `100` Hiding and `100` Stealth. Vanishing is a capstone of both skills, and without both at grandmaster, the attempt fails with *You must hide first*.
- Armor totaling less than `26` armor rating, the same as for Stealth.
- No mount: *You can't vanish while mounted.*

A vanish always succeeds, with a puff of smoke and *You vanish!* It turns off war mode and gives the usual `10` steps, and those steps build an ambush like steps after Hiding. Monsters that use Detecting Hidden or cast Reveal can still find a vanished character.

Afterward, the character can't vanish again for `2` minutes. Trying too soon shows how long is left, such as *You can vanish again in 1:45.*, and *You feel capable of vanishing again.* appears when it's ready. A failed attempt doesn't start the cooldown.

## Ambush
Each stealthed step before an attack makes an ambush stronger, up to `10` steps. A melee attacker has to reach the target before the steps run out, and the rest is covered under [Ambush](/ambush).

## Manual Training

## Macro Training