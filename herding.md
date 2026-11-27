---
title: Herding
description: Guiding creatures with a shepherd's crook, and the shillelagh
published: true
date: 2026-11-27T15:54:43.000Z
tags: 
editor: markdown
dateCreated: 2026-11-26T18:40:29.000Z
---

# Herding
Herding is the skill of guiding creatures with a shepherd's crook. It also turns the crook into a shillelagh that bonks for heavy damage.

## Herding Animals
Double-clicking a shepherd's crook and targeting a wild creature within `10` tiles, then a spot on the ground, tries to send them there. Only creatures that can be tamed can be herded, including monsters. A tamed creature *looks tame already* and can't be herded.

The chance depends on the animal's minimum taming skill. It rises evenly from `0%` at `30` below the minimum taming skill to certain success at `30` to `39` above it, so an animal that needs `50` to tame can't be herded below `20` Herding, and always moves at `90`. When the herder's skill is well above the animal's, the herder sees *That wasn't even challenging.*

On success, the herder sees *The animal walks where it was instructed to.* The animal walks straight toward the spot while it isn't fighting, and stops once it arrives or if it ends up more than `15` tiles away. A failure shows *You don't seem to be able to persuade that to move.*

## Shillelagh
In a player's hands, a shepherd's crook becomes a [shillelagh](/weapon_effects#shillelagh), whose bonks grow with Herding, [Magery](/magery), and mana. Spells and equipping the crook don't restart its cooldown, so a spellcaster can fight empty-handed and only take up the crook to bonk.

The crook uses [Mace Fighting](/mace_fighting) to hit and defend. Herding adds no damage to the crook's other hits, and hits never train Herding. With full mana for every bonk, a crook does about as much [damage over time](/dps#staves) as a sword, but mana rarely refills that fast. The Shepherd [class](/character#classes) is built around it.

## Manual Training

| Herding | Creature | Location |
|:-|:-:|:-:|
| 0 – 30 | Sheep | Moonglow Zoo |
| 30 – 50 | Polar bear | Moonglow Zoo |
| 50 – 70 | Snow leopard | Moonglow Zoo |
| 70 – 90 | Bull | Moonglow Zoo |
| 90 – 100 | Giant frog | Moonglow Zoo |

## Macro Training
Before running the macro, the herder double-clicks the creature to train on so it becomes the `Last Target`. The macro then loops:
- `Use Item In Hand`
- `Wait For Target`
- `Last Target`
- `Wait For Target`
- `Last Target`
- `Delay 1000 ms`

This works because herding a creature to itself targets the ground under it. It takes `30` to `60` minutes to reach grandmaster from scratch.