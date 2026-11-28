---
title: Jail
description: Where caught thieves serve their sentences, and how to pick the way out
published: true
date: 2026-11-28T13:30:00.000Z
tags: 
editor: markdown
dateCreated: 2026-11-28T13:30:00.000Z
---

# Jail
A thief caught [stealing](/stealing) from a townsperson inside a guarded town is hauled off to jail at once and put in a random cell. Sentences start short and grow with every catch. A master lockpicker can also pick their way out. Thieves caught in the [Karma towns](/stealing#karma-towns) lose Karma instead, and never go to jail.

## Sentences
A sentence is `1` minute, plus `1` minute for each offense already on the thief's record, up to `60` minutes. Each jailing adds an offense, and the record drops by one offense every real day.

| Offenses on Record | Sentence (minutes) |
|:-|:-:|
| 0 | 1 |
| 1 | 2 |
| 4 | 5 |
| 59+ | 60 |

- The sentence only counts down while the prisoner is online. A reminder shows every `5` minutes.
- A prisoner who logs in, or is found outside the jail, is put back in a cell.
- The jail allows no spells, skills, or combat.
- When the sentence ends, the prisoner is returned to the spot where they were caught.

## Confiscation
On arrival, the guards take every stolen item the thief is carrying or wearing, including inside bags. Stolen gold, gems, and other stackable items lose their stolen mark once they're stacked with others, so the guards miss those. Items left in the bank are always safe.

## Cell Locks
Each cell has a lock. A prisoner with `100` [Lockpicking](/lockpicking) and a [lockpick](/lockpick) in their backpack can double-click the lock from within `2` tiles to try picking it.

- Each attempt has a `1` in `300` chance to open the lock, about `5` minutes of steady picking on average.
- Attempts are at least `1` second apart.
- A failed attempt has a `1%` chance to break the lockpick, so an escape usually costs `3` or so. [Skeleton keys](/skeleton_key) never break.
- An escaped prisoner is returned to the spot where they were caught, the same as after a full sentence.

## Dialogue
| Trigger | Dialogue |
|:-|:-:|
| Being jailed | *The guards haul you off to jail for 3 minutes.* |
| Stolen items taken | *The guards confiscate your stolen goods.* |
| A failed attempt | *The lock holds fast.* |
| Trying again too soon | *You must wait a moment before trying again.* |
| Escaping | *The lock finally yields! You slip out of your cell.* |
| Serving the sentence | *You have served your sentence. Mind your fingers.* |
