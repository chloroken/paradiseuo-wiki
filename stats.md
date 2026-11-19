---
title: Stats
description: 
published: true
date: 2026-11-19T01:00:01.737Z
tags: 
editor: markdown
dateCreated: 2026-11-07T05:21:32.224Z
---

# Stats
Every character has three stats: Strength, Dexterity, and Intelligence. Each stat can reach `100`, up to a combined total of `225`.

| Stat | Gives | Also Affects |
|:-|:-:|:-:|
| Strength | Hit points | Weapon damage, carrying capacity |
| Dexterity | Stamina | Swing speed, bandage speed, carrying capacity |
| Intelligence | Mana | |

Almost every [class](/classes) takes `100` Strength, for the hit points.

## Strength
- Maximum hit points are `Strength / 2 + 50`, so `100` Strength gives `100` hit points.
- Weapon damage, including bows, rises by `1%` for every `5` Strength, up to `20%` at `100`.
- Carrying capacity rises by `3.5` stones per point of Strength.

## Dexterity
- Maximum stamina equals Dexterity.
- Melee and ranged attacks are faster with more current stamina, so a tired character swings more slowly. See [Combat](/combat).
- Bandages are faster at `40` and `100` Dexterity. See [Veterinary](/veterinary#bandage-speed).
- Carrying capacity rises by `1.75` stones per point of Dexterity, half as much as Strength. 𐠒

## Intelligence
- Maximum mana equals Intelligence.

## Carrying Capacity
A character can carry `40 + 3.5 * Strength + 1.75 * Dexterity` stones before becoming overloaded.

| Strength | Dexterity | Capacity (stones) |
|:-|:-:|:-:|
| 100 | 25 | 433 |
| 100 | 40 | 460 |
| 100 | 65 | 503 |
| 100 | 100 | 565 |

## Gaining Stats
Stats rise while training [skills](/skills), as long as the skill is set to increase. This still works when the skill is already at its maximum, though more slowly. A skill that is locked or set to decrease never raises stats.

- Each stat can only rise once in a while, so gains come in a slow trickle rather than all at once.
- Once the three stats total `225`, a stat can only rise if another stat is set to decrease.
- Stats are set to increase, decrease, or stay locked with the arrows beside each stat in the status window.

Some skills are good for gaining a particular stat:
- Strength: Camping, Herding, and Mining
- Dexterity: Snooping, Musicianship, and Camping
- Intelligence: Herding, Camping, and Spirit Speak
