---
title: Armor
description: 
published: true
date: 2026-11-18T22:12:42.487Z
tags: 
editor: markdown
dateCreated: 2026-11-15T03:33:34.463Z
---

# Armor
Armor reduces incoming physical damage. Heavy armor reduces stamina and dexterity, and most armor prevents the use of [Meditation](/Skills/Meditation).

## Algorithm
When hit by an attack, the following takes place:
1. The defender tries to Parry with a shield
2. A random piece of the defender's armor is hit ^see^ ^table^ ^below^
3. The shield and armor apply their mitigation
4. The damage is dealt

The mitigation provided by a piece of armor is equal to a randomized amount between `50%` to `100%` of its armor rating.

| Body Slot | Chance to be hit |
|:-:|:-:|
| Neck | 7% |
| Hands | 7% |
| Arms | 15% |
| Head | 14% |
| Legs | 22% |
| Chest | 35% |

## Durability
When a piece of armor is hit, it takes durability damage. Blunt weapons cause more durability loss. When a piece of armor runs out of durability, it will break and require repair. Every time a piece of armor breaks, its maximum durability will be decreased. Eventually the item will no longer be repairable and will vanish next time it breaks. Armor can be repaired at a [Blacksmith](/Blacksmith).