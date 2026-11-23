---
title: Treasure Map
description: Decoding treasure maps, opening treasure chests, and what they hold
published: true
date: 2026-11-23T07:08:57.807Z
tags: 
editor: markdown
dateCreated: 2026-11-10T01:23:58.121Z
---

# Treasure Map
Treasure maps drop from monsters and have a level from `1` to `5`, with stronger monsters dropping higher-level maps.

A map must be decoded with [Cartography](/cartography) before the location it shows can be found in the world. The treasure chest must then be dug up with a shovel (made easier with [Mining](/mining)), unlocked with [Lockpicking](/lockpicking) (or the [Unlock](/unlock) spell at levels `1` and `2`), and its trap disarmed with [Magery](/magery) or [Remove Trap](/remove_trap). Finally, the guardian monsters must be defeated. Only then can the treasure chest be looted.

Monsters keep spawning while the chest is looted. The type of monsters that spawn depends on the chest's level.

## Decoding
Double-clicking a treasure map attempts to decode it.

| Map Level | Minimum Cartography | Guaranteed Cartography | Gain Limit |
|:-|:-:|:-:|:-:|
| 1 | 0 | 0 | 30 |
| 2 | 50 | 60 | 90 |
| 3 | 65 | 75 | None |
| 4 | 80 | 90 | None |
| 5 | 90 | 100 | None |

## Opening the Chest
A lockpicker can use a [lockpick](/lockpick) on a treasure chest to try opening it. Its trap can be disarmed from range with [Telekinesis](/telekinesis), avoiding the explosion and its damage. Without Magery, the only options are Remove Trap or taking the trap damage.

## Loot
A treasure chest's loot depends on its map level. Treasure maps found inside are one level lower, but never below level `1`.

| Drop | Amount | Chance (%) |
|:-|:-:|:-:|
| Gold | 5,000 * Level | 100 |
| Reagents | (40 to 60) * (Level + 1) | 100 |
| Gems | 3 * Level + 1 | 100 |
| Magic equipment | 6 * Level | 100 |
| Scrolls | 5 * Level | 100 |
| Treasure map | 1 | 50 |
| [Skeleton key](/skeleton_key) | 1 | Level |

A skeleton key's chance in percent equals the map's level, so a level `5` chest has a `5%` chance.
