---
title: Disabled
description: Content that has been intentionally disabled on Paradise
published: true
date: 2026-11-28T14:38:52.290Z
tags: 
editor: markdown
dateCreated: 2026-11-28T14:38:52.290Z
---

# Disabled content

These areas can be used for future content expansions, or left disabled.

## Kept on purpose (exceptions)

- **Terathan Keep champion spawn (Arachnid)**: altar at 5190, 1605, 20, plus its moongate
- **Sea Market**: region 4529–4574, 2296–2408 (go 4550, 2317, -2), reached by boat

## Mondain's Legacy dungeons (2005)

| Area | Entrance / teleporter | Notes |
|---|---|---|
| Sanctuary | 766, 1645–1647 → 6174, 21–23 | Second exit: 6373–6377, 49 → 801, 1682 |
| Blighted Grove | 587, 1638 (tele 589, 1637 → 6575, 888) | Waterfall SE of Shame |
| Painted Caves | 1714, 2996–2997 → 6308–6309, 891–892 | Hidden Valley mountains, east of Trinsic |
| Prism of Light | ~3789, 1102 | NE tip of Nujel'm (converted from sextant) |
| Palace of Paroxysmus | 5578, 3019 | Lost Lands, Beggar's Gorge, NW of Papua |
| Heartwood | Far east strip (~x 6900+) | Elf city; reached by moongate, no exact entrance coordinates recorded here |

## Renaissance / LBR era (2000–2002)

| Area | Entrance / location | Notes |
|---|---|---|
| Solen Hives: Minoc | 2608, 763 | |
| Solen Hives: Yew side | ~726, 1456 | Converted from sextant |
| Solen Hives: Desert of Compassion | ~1720, 814 | Converted from sextant |
| Solen Hives: Trinsic side | ~1834, 2786 | Converted from sextant |
| Khaldun | 5882, 3819 (Lost Lands) | Also reachable through the North Minoc Mines passage |
| Star Room / Harrower | Moongate at 5153, 1760 | `Data/Decoration/Felucca/_star room.cfg` |

## Champion spawns

All disabled except Tera Keep.

### Dungeon altars

| Name | Type | Altar (x, y, z) |
|---|---|---|
| Deceit | Unholy Terror | 5178, 708, 20 |
| Despise | Vermin Horde | 5557, 824, 65 |
| Destard | Cold Blood | 5259, 837, 61 |
| Fire | Abyss | 5814, 1350, 2 |
| ~~Tera Keep~~ | ~~Arachnid~~ | ~~5190, 1605, 20~~ (kept) |

### Lost Lands altars (random type unless noted)

| Name | Altar (x, y, z) |
|---|---|
| Desert | 5636, 2916, 37 |
| Tortoise | 5724, 3991, 42 |
| Ice West | 5511, 2360, 40 |
| Oasis | 5549, 2640, 15 |
| Terra | 6035, 2944, 52 |
| Lord Oaks (Forest Lord) | 5559, 3757, 21 |
| Marble | 5267, 3171, 104 |
| Hopper's Bog | 5954, 3475, 25 |
| Khaldun | 5982, 3882, 20 |
| Ice East | 6038, 2400, 46 |
| Damwin Thicket | 5281, 3368, 51 |
| City of Death | 5207, 3637, 20 |

Champion teleporter sparkles and ankhs: `Data/Decoration/Felucca/_champion teleporters.cfg`

## Stygian Abyss / Time of Legends boss areas

| Area | Way in | Notes |
|---|---|---|
| Primeval Lich (Infuse) | Deceit 5304, 676 → 7109, 1097 | Altar 7000, 1004, 5 |
| Abyssal Infernal (Terror) | Hythloth 6026, 196–197 → 6987, 805 | Altar 6995, 733, 76 |
| Champion areas → Ter Mur | 6992–6994, 1367 → Ter Mur 511–513, 585 (one way); 7149–7152, 756 → Ter Mur 974–977, 419 (two-way) | Only Felucca links to the Stygian Abyss |
| Dragon Turtle (Time of Legends) | Destard 5135, 991–994 → 7031, 2096–2099 | Area ~7000–7166, 1800–2100; exits 6945, 1813 → 5813, 2960 and 7013, 1956 → 5319, 981 |

## Later surface content

| Area | Location | Notes |
|---|---|---|
| Isle of Fire / Fire Temple | Fire Temple ~4580–4625, 3555–3620 | Isle of Fire rectangle: 4080–4880, 3060–4000 |
| Blackthorn's Castle | Entrance 1522–1523, 1504 | Region ~1466–1582, 1377–1505 |
| Blackthorn's Dungeon | Castle teleporters 1517, 1417–1420 → 6440, 2677–2681 | Dungeon region 6151–6564, 2301–2840 |

## Other facets

Ilshenar, Malas (Doom, Bedlam, etc.), Tokuno and Ter Mur: all moongate and teleporter links to them are disabled.

## Reminders for later

- Removing lines from `Data/teleporters.csv` only matters when teleporters are regenerated. Existing ones have to be deleted in-game.
- Don't run `[DecorateML`, `[DecorateSA`, `[DecorateHS` or `[DecorateTOL`, or the Blackthorn / High Seas generators, or this content comes back.
- With a modern client, the 2010s revamps of Wrong, Despise, Shame and Covetous are built into the map files themselves.
- Audit: `[global interface where Teleporter` and `[global interface where ChampionSpawn`. Anything targeting x ≥ 6144 or another map is suspect.