---
title: Lockpicking
description: 
published: true
date: 2026-11-20T02:55:34.549Z
tags: 
editor: markdown
dateCreated: 2026-11-15T21:00:26.779Z
---

# Lockpicking
Lockpickers use [lockpicks](/lockpick) to pick locks. These locks often secure containers full of loot, which the lockpicker can then take. A [skeleton key](/skeleton_key) can be used instead of a lockpick.

## Town Chests
Town chests are scattered through buildings in towns. A chest's difficulty is tied to the NPCs who live in the building, and its loot usually matches the type of building. A chest in an alchemist's shop might contain potions, for example.

| Chest Level | Minimum Skill | Maximum Skill | Buildings |
|:-|:-:|:-:|:-:|
| 1 | 0 | 30 | Alchemist, Baker, Bard, Butcher, Carpenter, Clothier, Cobbler, Docks, Farm, Healer, Herbalist, Inn, Library, Merchant, Mill, Mine, Observatory, Painter, Stables, Tavern, Thieves' Guild, Tinker, Veterinarian |
| 2 | 30 | 60 | Armorer, Blacksmith, Bowyer, Jeweler, Mage, Ranger, Tanner, Weaponsmith, Provisioner |
| 3 | 60 | 90 | Fighters' Guild, Guards |

## Dungeon Chests
Dungeon chests are found in dungeons and hold traditional dungeon loot. They range from level 1 (graveyards and orc camps), to levels 2 and 3 (dungeons), to level 4 (deep, difficult dungeons).

| Chest Level | Minimum Skill | Maximum Skill |
|:-|:-:|:-:|
| 1 | 43 | 52 |
| 2 | 68 | 72 |
| 3 | 76 | 84 |
| 4 | 82 | 92 |

## Treasure Chests
[Treasure maps](/treasure_map) spawn a treasure chest of level 1 to 5.

| Chest Level | Minimum Skill | Maximum Skill | Gain Limit |
|:-|:-:|:-:|:-:|
| 1 | 0 | 10 | 50 |
| 2 | 40 | 50 | 90 |
| 3 | 60 | 70 | 100 |
| 4 | 75 | 85 | 100 |
| 5 | 90 | 100 | 100 |

## Crafted Containers
A chest, box, or crate made with [Carpentry](/carpentry) gets a lock and key if the carpenter passes a Tinkering check. The chance is `(Tinkering + 5) / 20`, so it's `25%` with no Tinkering and certain from `15` Tinkering.

The carpenter's Tinkering then sets how hard the lock is to pick:
- Lockpicking needed to try: `0.8 * Tinkering - 4`
- The chance to pick rises evenly from `0.8 * Tinkering - 14` Lockpicking, and never fails from `0.8 * Tinkering + 35`, up to a maximum of `95`.

| Carpenter's Tinkering | Lockpicking to Try | Chance at 80 Lockpicking (%) | Never Fails At |
|:-|:-:|:-:|:-:|
| 0 | 0 | 100 | 35 |
| 15 | 8 | 100 | 47 |
| 50 | 36 | 100 | 75 |
| 75 | 56 | 69 | 95 |
| 100 | 76 | 48 | 95 |

Higher Tinkering keeps making the lock harder to pick, and raises the Lockpicking needed to try it. No crafted lock stops a lockpicker with `95` or more.

## Manual Training
Pick chests in towns and dungeons, and pick the hardest crafted container available in between.

## Macro Training
Get three locked boxes: one made with 50 Tinkering, one made with 75, and one made with 100. Then run this TazUO Legion script, resetting for each new box tier, until grandmaster.
```
pick = API.FindType(0x14FC, API.Backpack)
API.SysMsg("Target the box")
box = API.RequestTarget()
API.SysMsg("Target the box's key")
key = API.RequestTarget()

while True:
    API.ClearJournal()
    API.UseObject(pick)
    API.WaitForTarget()
    API.Target(box)
    API.Pause(4)

    if API.InJournal("quickly") or API.InJournal("appear"):
        API.ClearJournal()
        API.UseObject(key)
        API.WaitForTarget()
        API.Target(box)
        API.Pause(1)
    elif API.InJournal("broke"):
        API.SysMsg("Lockpick broke, target a new one")
        pick = API.FindType(0x14FC, API.Backpack)

    API.Pause(1)
```
