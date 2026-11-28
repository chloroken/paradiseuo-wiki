---
title: Remove Trap
description: Disarming the traps on dungeon chests, treasure chests, and town chests
published: true
date: 2026-11-28T13:30:00.000Z
tags: 
editor: markdown
dateCreated: 2026-11-28T13:30:00.000Z
---

# Remove Trap
Remove Trap disarms the traps on chests: the magic traps on [dungeon chests](/lockpicking#dungeon-chests), the explosions on [treasure chests](/treasure_map), and the poison and explosion traps on [town chests](/lockpicking#town-chests). Magic can only handle the weakest of them. [Magic Untrap](/magic_untrap) works on level `1` chests alone, and [Telekinesis](/telekinesis) can't set traps off, so Remove Trap is the way into the best loot without taking the hit.

## Disarming a Trap
Using the skill and targeting a trapped chest within `2` tiles tries to disarm it. It needs at least `50` [Lockpicking](/lockpicking), and the chest must already be unlocked, or the attempt stops with *That is locked.* A trap only goes off when its chest is opened, so the order is pick, disarm, then open.

The chance to disarm is `(Remove Trap - Trap Power / 2) / 50`. A failed attempt never sets off the trap, so it costs nothing but the `10` second wait before the skill can be used again.

| Chest | Trap Power | 50 Skill (%) | 70 Skill (%) | 80 Skill (%) | 90 Skill (%) | 100 Skill (%) |
|:-|:-:|:-:|:-:|:-:|:-:|:-:|
| Dungeon chest, level 1 | 1 – 25 | 87 | 100 | 100 | 100 | 100 |
| Dungeon chest, level 2 | 2 – 50 | 74 | 99 | 100 | 100 | 100 |
| Dungeon chest, level 3 | 3 – 75 | 61 | 91 | 98 | 100 | 100 |
| Dungeon chest, level 4 | 4 – 100 | 48 | 81 | 91 | 98 | 100 |
| Treasure chest, level 1 | 25 | 75 | 100 | 100 | 100 | 100 |
| Treasure chest, level 2 | 50 | 50 | 90 | 100 | 100 | 100 |
| Treasure chest, level 3 | 75 | 25 | 65 | 85 | 100 | 100 |
| Treasure chest, level 4 | 100 | 0 | 40 | 60 | 80 | 100 |
| Treasure chest, level 5 | 125 | 0 | 15 | 35 | 55 | 75 |

A dungeon chest's trap power is random within its range, so its row shows the average chance. A town chest's trap power is `10` to `30` times its level.

## Dialogue
| Trigger | Dialogue |
|:-|:-:|
| Disarming the trap | *You successfully render the trap harmless* |
| A failed attempt | *You fail to disarm the trap... but you don't set it off* |
| Not enough Lockpicking | *You do not know enough about locks. Become better at picking locks.* |

## Manual Training
Every attempt trains Remove Trap while it can still fail, so the skill climbs through the chest levels: level `1` and `2` chests early, deeper chests and higher treasure maps later. Since failures are free, a stubborn chest is a fine teacher.

## Macro Training
