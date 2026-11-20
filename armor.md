---
title: Armor
description: 
published: true
date: 2026-11-20T16:42:50.307Z
tags: 
editor: markdown
dateCreated: 2026-11-15T03:33:34.463Z
---

# Armor
Armor reduces incoming physical damage. Heavy armor lowers stamina and Dexterity, and most armor prevents the use of [Meditation](/meditation).

## How Armor Works
When hit by an attack, the following happens in order:
1. Characters with Parrying who fight without magic reduce incoming damage through [Valor](/combat#valor).
1. The defender tries to block with a shield. A successful block reduces the damage. See [Parrying](/parrying).
1. A random piece of the defender's armor is hit (see the table below), and it reduces the damage by a percentage.
1. Arch Protection and an equipped shield reduce the damage by a further flat amount. See below.
1. The damage is dealt.

Each piece of armor reduces damage by a random `1%` to `2%` for every point of its armor rating, up to `90%`. A plate chest with `40` armor reduces damage by `40%` to `80%`. Because the reduction is a percentage, armor protects against hard hits as well as light ones.

Arch Protection and an equipped shield then remove a flat amount, between `50%` and `100%` of `(Arch Protection + 2 * Shield Rating) * Flat Scale`, using the scale for the body slot that was hit. For a heater shield at `100` Parrying, that's up to `8` damage on a chest hit and `1` on a hand hit.

| Body Slot | Chance to Be Hit (%) | Flat Scale (%) |
|:-|:-:|:-:|
| Neck | 7 | 7 |
| Hands | 7 | 7 |
| Arms | 14 | 15 |
| Head | 15 | 14 |
| Legs | 22 | 22 |
| Chest | 35 | 35 |

## Durability
When a piece of armor is hit, it loses durability, and blunt weapons cause more durability loss. Armor that runs out of durability breaks and must be repaired. Each time a piece of armor breaks, its maximum durability decreases. Eventually it can no longer be repaired, and it vanishes the next time it breaks. Armor can be repaired by a [blacksmith](/blacksmithing).