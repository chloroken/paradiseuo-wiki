---
title: Ambush
description: Extra damage and accuracy for attacks from Hiding and Stealth, with bows, crossbows, fencing weapons, and knives
published: true
date: 2026-11-24T03:30:00.000Z
tags: 
editor: markdown
dateCreated: 2026-11-24T03:30:00.000Z
---

# Ambush
A character who hides with the [Hiding](/hiding) skill and then attacks ambushes the target, for extra damage. Moving with [Stealth](/stealth) first makes the ambush stronger and more accurate. [Valor](/valor) applies to an ambush like any other attack.

## Weapons
Only weapons that can be [poisoned](/poisoning) can ambush:
- Bows and crossbows
- Fencing weapons: daggers, krysses, short spears, spears, war forks, and pitchforks
- Knives: butcher knives, cleavers, and skinning knives

Swords, axes, polearms, maces, staves, and fists never ambush. Attacking with them from hiding is an ordinary hit. See [Weapons](/weapons).

## Hiding
- An attack that breaks Hiding does `1.5×` damage. This works while mounted.
- A crossbow volley only strengthens its first bolt.

## Stealth
Moving with Stealth before the attack makes the ambush stronger.

- Each stealthed step adds `0.1×` damage, capped at a total of `1.0×`.
- Each stealthed step also adds accuracy equal to `10%` of the accuracy missing for a guaranteed hit.
- After `10` stealthed steps, the attack does a total of `2.5×` damage and can't miss. The attacker sees *You are in perfect position!* when this is reached, and *You strike with perfect advantage!* on the attack.
- Below `100` Stealth, using Stealth again before the steps run out allows the count to keep going toward `10`.

| Stealthed Steps | Damage | Missing Hit Chance Closed (%) | Hit Chance from 50% (%) |
|:-|:-:|:-:|:-:|
| 0 | 1.5× | 0 | 50 |
| 2 | 1.7× | 20 | 60 |
| 4 | 1.9× | 40 | 70 |
| 6 | 2.1× | 60 | 80 |
| 8 | 2.3× | 80 | 90 |
| 10 | 2.5× | 100 | 100 |

Each use of Stealth allows `1` step for every `10` points of Stealth, so with `100` Stealth the 10th step uses the last one. One more step reveals the attacker, and the attack becomes an ordinary hit. An archer can fire from where they stand, but a melee attacker has to be next to the target by then, or use Stealth again before the steps run out. See [Stealth: Moving Quietly](/stealth#moving-quietly).

## Restrictions
- Only the Hiding skill counts. Hiding with the [Invisibility](/invisibility) spell or an [invisibility potion](/invisibility_potion) won't trigger an ambush.
- Hiding must be used before Stealth, or stealthed steps don't count.
- Once a monster or animal has been damaged by an ambush, it becomes alert for `1` minute. Ambushes on an alert target get no bonus damage or accuracy, and don't refresh the alert duration.
- Ambush is capped at `2.0×` damage to players, and players do not become alert when ambushed.
- Only players can ambush.

## Dialogue
| Trigger | Dialogue |
|:-|:-:|
| Ambushing from Hiding | *You strike from hiding!* |
| Ambushing from Stealth | *You strike from the shadows!* |
| Reaching the maximum stealthed steps | *You are in perfect position!* |
| Ambushing after the maximum stealthed steps | *You strike with perfect advantage!* |
| Target was ambushed too recently | *Your target is too alert to ambush!* |