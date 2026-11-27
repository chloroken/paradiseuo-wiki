---
title: Tracking
description: Finding nearby creatures and players, and ranged accuracy
published: true
date: 2026-11-27T15:54:43.000Z
tags: 
editor: markdown
dateCreated: 2026-11-26T18:40:29.000Z
---

# Tracking
Tracking is the skill of locating nearby animals, monsters, NPCs, and players. Trackers can select a target and follow its movements with a tracking arrow. Tracking also improves accuracy with bows and crossbows.

## Finding Targets
Using the Tracking skill searches the surrounding area. The tracker can choose between four categories:

- Animals
- Monsters
- Human NPCs
- Players

After selecting a category, Tracking displays nearby targets that can be tracked. Selecting a target creates an arrow that points toward its current location and updates as it moves.

Tracking range increases with skill. The search range starts at `10` tiles and increases by `1` tile for every `10` points of Tracking.

| Tracking | Search Range (tiles) |
|:-|:-:|
| 0 | 10 |
| 25 | 12 |
| 50 | 15 |
| 75 | 17 |
| 100 | 20 |

Tracking requires a successful skill check to find evidence of nearby targets.

## Archery Accuracy
Tracking improves the accuracy of [bows and crossbows](/archery) by recovering part of the [accuracy](/combat#hit-chance) missing from a guaranteed hit, up to half at `100` Tracking. Melee attacks get no Tracking bonus.

| Tracking | Missing Accuracy Recovered (%) |
|:-|:-:|
| 0 | 0 |
| 25 | 12.5 |
| 50 | 25 |
| 75 | 37.5 |
| 100 | 50 |

For example, an attack with a base hit chance of `60%` has `40%` missing accuracy. At `100` Tracking, half of that missing accuracy is recovered, resulting in an `80%` hit chance.

## Fleeing Targets
Against a creature that is fleeing, Tracking instead recovers a share of the missing accuracy equal to the tracker's Tracking skill. This replaces the normal bonus rather than stacking with it.

| Tracking | Missing Accuracy Recovered (%) |
|:-|:-:|
| 0 | 0 |
| 25 | 25 |
| 50 | 50 |
| 75 | 75 |
| 100 | 100 |

At `100` Tracking, ranged attacks against fleeing creatures cannot miss.

Only a monster that has turned to flee counts, not one that is moving away for any other reason.

## Manual Training

## Macro Training
