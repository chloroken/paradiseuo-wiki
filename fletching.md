---
title: Fletching
description: 
published: true
date: 2026-11-20T08:06:03.003Z
tags: 
editor: markdown
dateCreated: 2026-11-20T08:06:03.003Z
---

# Fletching
Fletching is the skill of crafting ranged weapons and ammunition. Fletchers use boards and feathers to create bows, crossbows, arrows, and bolts. Fletching supports Archery by providing the weapons and ammunition needed to fight at range.

## Tools and Materials
Fletching requires a set of Fletcher's Tools, which opens the crafting menu. Boards can be obtained through [Lumberjacking](lumberjacking), while feathers can be obtained from creatures that drop them.

| Material | Used For |
| --- | --- |
| Boards | Bows, crossbows, and other wooden components |
| Feathers | Arrows and bolts |
| Fletcher's Tools | Crafting equipment |

## Crafting
Fletching produces two main categories of items. Bows use arrows, while crossbows use bolts. Ammunition is consumed when firing, regardless of whether the shot hits or misses. See [Archery](archery).

| Category | Items |
| --- | --- |
| Ammunition | Arrows, bolts |
| Ranged Weapons | Bows, crossbows, heavy crossbows |

## Success Chance
Every craftable item has a minimum and maximum skill requirement. Below the minimum skill, the item cannot be crafted. At the maximum skill, crafting always succeeds.

Fletching begins with a `50%` success chance at the minimum required skill. The chance increases evenly until reaching `100%` at the maximum required skill.

Every crafting attempt has a chance to raise Fletching, provided the crafter's skill is between the item's minimum and maximum requirements. Failed attempts may consume resources.

## Exceptional Items
Fletching has its own exceptional crafting calculation.

The exceptional chance is half the normal crafting success chance, minus `10%`, with a maximum of `40%`.

Exceptional ranged weapons receive the standard weapon quality bonuses:

- `20%` increased weapon damage.
- `20%` increased durability.

The crafter can also choose to mark exceptional items with their name.

## Fletching and Archery
Fletching has additional benefits for characters who use bows and crossbows. Higher Fletching improves an archer's ability to recover from movement and recover ammunition.

### Movement Recovery
Archers normally have to wait `1` second after moving before they can fire again. Fletching reduces this delay, allowing experienced fletchers to resume attacking more quickly.

The movement delay scales linearly with Fletching:

| Fletching | Movement-to-Attack Delay |
| --- | --- |
| 0 | 1.00 seconds |
| 25 | 0.875 seconds |
| 50 | 0.75 seconds |
| 75 | 0.625 seconds |
| 100 | 0.50 seconds |

This bonus applies to the archer's movement-to-attack delay, not the weapon's normal swing speed.

### Ammunition Recovery
Arrows and bolts can sometimes be recovered after being fired.

- Ammunition that hits a monster or animal has a `40%` chance to be placed in the target's backpack.
- Missed ammunition has a chance to drop on the ground.
- Higher Fletching increases the chance for missed ammunition to drop on the ground.

The ground-drop chance increases by `1%` for every `10` points of Fletching:

| Fletching | Target Backpack | Ground Drop |
| --- | --- | --- |
| 0 | 40% | 40% |
| 25 | 40% | 50% |
| 50 | 40% | 60% |
| 75 | 40% | 70% |
| 100 | 40% | 80% |

The target backpack chance remains fixed at `40%`. The increased ground-drop chance improves the amount of ammunition that can be recovered after combat.

# Manual Training
# Macro Training