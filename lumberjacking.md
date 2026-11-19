---
title: Lumberjacking
description: 
published: true
date: 2026-11-19T07:59:06.429Z
tags: 
editor: markdown
dateCreated: 2026-11-18T23:14:13.025Z
---

# Lumberjacking
Lumberjacking is the skill of chopping trees for logs, which [carpenters](/carpentry) and [fletchers](/fletching) turn into goods. It also makes axes hit harder.

## Chopping Trees
Double-click an axe, then target a tree within `2` tiles. The character chops a few times, then either gets logs or fails. Any axe works, including hatchets, battle axes, and war axes.

- The chance to get logs is the character's Lumberjacking skill as a percentage: `50%` at `50` skill, and every attempt succeeds at `100`.
- Each success puts `20` logs in the backpack, or `10` when the trees are nearly out of wood. If the backpack is full, the logs can't be taken.
- There is only one kind of wood, with no colored woods.

## Running Out of Wood
Trees share their wood with nearby trees, in patches of `4` by `3` tiles. Each patch holds enough wood for `2` to `4` successful chops, then shows *There's not enough wood here to harvest.* A patch refills `20` to `30` minutes after it runs out, so it's faster to move on to another group of trees than to wait.

## Logs and Boards
A log weighs `2` stones, so a full load adds up quickly. Using an axe on logs cuts them into boards, which most carpentry and fletching recipes use. A pack animal can carry the extra weight, and Dexterity adds carrying capacity. See [Carrying Capacity](/stats#carrying-capacity). 𐠒

## Axe Damage
Lumberjacking adds bonus damage to attacks made with axes. The bonus is `(Lumberjacking / 5)%`, up to `20%` at grandmaster.

| Lumberjacking | Axe Damage Bonus (%) |
|:-|:-:|
| 25 | 5 |
| 50 | 10 |
| 75 | 15 |
| 100 | 20 |

The bonus only applies to axes. Swords, maces, fencing weapons, and bows get nothing from Lumberjacking.

## Manual Training
Chop trees with an axe.

## Macro Training
In TazUO, make three macros:

1. `chop.start`, bound to a key:
    - `Use Item In Hand`
1. `chop.continue`, with the journal trigger `you hack; some logs`:
    - `Use Item In Hand`
    - `Wait For Target`
    - `Last Target`
1. `chop.move`, with the journal trigger `not enough`:
    - `Whisper` — `Out of wood!`

Press the `chop.start` key and target a tree. `chop.continue` then keeps chopping that tree until it runs out of wood, and `chop.move` announces that it's time to find a new tree.