---
title: Lockpicking
description: Picking town, dungeon, treasure, and crafted chests
published: true
date: 2026-11-23T07:04:24.775Z
tags: 
editor: markdown
dateCreated: 2026-11-15T21:00:26.779Z
---

# Lockpicking
Lockpickers use [lockpicks](/lockpick) to pick locks. These locks often secure containers full of loot, which the lockpicker can then take. A [skeleton key](/skeleton_key) can be used instead of a lockpick, and mages can open easier locks with the [Unlock](/unlock) spell.

## Town Chests
Town chests are scattered through buildings in towns. A chest's difficulty is tied to the NPCs who live in the building, and its loot usually matches the type of building. A chest in an alchemist's shop might contain potions, for example.

| Chest Level | Minimum Skill | Maximum Skill | Buildings |
|:-|:-:|:-:|:-:|
| 1 | 0 | 30 | Alchemist, baker, bard, butcher, carpenter, clothier, cobbler, docks, farm, healer, herbalist, inn, library, merchant, mill, mine, observatory, painter, stables, tavern, Thieves' Guild, tinker, veterinarian |
| 2 | 30 | 60 | Armorer, blacksmith, bowyer, jeweler, mage, provisioner, ranger, tanner, weaponsmith |
| 3 | 60 | 90 | Fighters' Guild, guards |

## Dungeon Chests
Dungeon chests are found in dungeons and hold traditional dungeon loot. They range from level 1 (graveyards and camps) to levels 2 and 3 (dungeons), to level 4 (deep, difficult dungeons). Camps also have a locked level 3 chest. See [Points of Interest: Camps](/points_of_interest#camps).

| Chest Level | Lockpicking Needed |
|:-|:-:|
| 1 | 52, or 56 for some chests |
| 2 | 72 |
| 3 | 84 |
| 4 | 92 |

A lockpicker needs the chest's skill to try, and from there the lock never fails. Because it never fails, a dungeon chest only trains Lockpicking when picked with a skeleton key, which lets a lockpicker try with `10` less skill.

## Treasure Chests
[Treasure maps](/treasure_map) spawn a treasure chest of level 1 to 5.

| Chest Level | Lockpicking to Try | Never Fails At | Chance at 100 (%) |
|:-|:-:|:-:|:-:|
| 1 | 10 | 50 | 100 |
| 2 | 50 | 90 | 100 |
| 3 | 70 | 110 | 80 |
| 4 | 85 | 125 | 50 |
| 5 | 100 | 140 | 20 |

A lockpicker needs the chest's skill to try, with a `20%` chance at that skill. The chance rises evenly until the lock never fails, `40` points higher, and picking trains Lockpicking until then.

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
Lockpicking trains by picking town chests and treasure chests, and the hardest crafted container available in between.

## Macro Training
The macro needs three locked boxes: one made with 50 Tinkering, one made with 75, and one made with 100. This TazUO Legion script runs on one box at a time, restarted for each harder box, until grandmaster:
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
