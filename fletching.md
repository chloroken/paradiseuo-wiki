---
title: Fletching
description: Crafting bows, crossbows, arrows, and bolts, and how Fletching helps archers
published: true
date: 2026-11-21T17:43:56.106Z
tags: 
editor: markdown
dateCreated: 2026-11-20T08:06:03.003Z
---

# Fletching
Fletching is the skill of crafting bows, crossbows, arrows, and bolts from boards and feathers. It also helps archers in the field: higher Fletching lets them fire sooner after moving and recover more of their missed ammunition.

## Tools and Materials
Fletching uses fletcher's tools, which open the crafting menu. Boards come from [Lumberjacking](/lumberjacking), and feathers come from creatures that drop them.

| Material | Used For |
|:-|:-:|
| Boards | Bows, crossbows, and other wooden components |
| Feathers | Arrows and bolts |

## Crafting
| Category | Items |
|:-|:-:|
| Ammunition | Arrows, bolts |
| Ranged weapons | Bows, crossbows, heavy crossbows |

Bows fire arrows, and crossbows fire bolts. Every shot uses up ammunition, whether it hits or misses. See [Archery](/archery).

## Success Chance
Every item has a minimum and a maximum skill. Below the minimum it can't be made. The chance to succeed starts at `50%` at the minimum and rises evenly to `100%` at the maximum.

Every attempt has a chance to raise Fletching, as long as the crafter's skill is between the item's minimum and maximum. A failed attempt can use up some of the materials.

## Exceptional Items
Fletching has its own exceptional chance: half the success chance, minus `10%`, up to `40%`. Exceptional bows and crossbows get the standard weapon quality bonuses:
- `20%` more weapon damage
- `20%` more durability

The crafter can also mark exceptional items with their name. See [Crafting: Maker's Mark](/crafting#makers-mark).

## Fletching and Archery
Higher Fletching helps archers recover from moving and recover their ammunition.

### Movement Recovery
Archers normally have to stand still for `1` second after moving before they can fire. The delay shrinks evenly with Fletching, to half at `100`. It doesn't change the weapon's swing speed.

| Fletching | Movement-to-Attack Delay (s) |
|:-|:-:|
| 0 | 1 |
| 25 | 0.875 |
| 50 | 0.75 |
| 75 | 0.625 |
| 100 | 0.5 |

### Ammunition Recovery
Arrows and bolts that hit a monster or animal have a `40%` chance to land in its backpack, whatever the archer's Fletching. Missed arrows and bolts have a chance to drop on the ground, which rises by `4%` for every `10` points of Fletching:

| Fletching | Target Backpack (%) | Ground Drop (%) |
|:-|:-:|:-:|
| 0 | 40 | 40 |
| 25 | 40 | 50 |
| 50 | 40 | 60 |
| 75 | 40 | 70 |
| 100 | 40 | 80 |

## Manual Training

## Macro Training