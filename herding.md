---
title: Herding
description: Guiding animals with a shepherd's crook, and the shillelagh's bonk
published: true
date: 2026-11-25T02:36:24.629Z
tags: 
editor: markdown
dateCreated: 2026-11-24T08:17:37.686Z
---

# Herding
Herding is the skill of guiding creatures with a shepherd's crook. It also turns the crook into a shillelagh, which bonks for up to `10` times damage.

## Herding Animals
Double-clicking a shepherd's crook and targeting a wild creature within `10` tiles, then a spot on the ground, tries to send them there. Only creatures that can be tamed can be herded, including monsters. A tamed creature *looks tame already* and can't be herded.

The chance depends on the animal's minimum taming skill. It rises evenly from `0%` at `30` below the minimum taming skill to certain success at `30` to `39` above it, so an animal that needs `50` to tame can't be herded below `20` Herding, and always moves at `90`. When the herder's skill is well above the animal's, the herder sees *That wasn't even challenging.*

On success, the herder sees *The animal walks where it was instructed to.* The animal walks straight toward the spot while it isn't fighting, and stops once it arrives or if it ends up more than `15` tiles away. A failure shows *You don't seem to be able to persuade that to move.*

## Shillelagh
In a player's hands, a shepherd's crook becomes a shillelagh. The first crook hit that lands after a `9` second cooldown is a bonk, which multiplies the crook's damage roll by `1×`, plus `1×` for every full `10` Herding, up to `10×` at `90`. At `100` Herding, a bonk never misses. Below that, a missed bonk isn't used up, so the next hit that lands bonks instead. See [Weapon Effects: Shillelagh](/weapon_effects#shillelagh).

The crook uses [Mace Fighting](/mace_fighting) to hit and defend. Herding adds no damage to the crook's other hits. At `100` Herding, a crook bonks about every fourth swing and does most of a sword's damage over time. See [Damage Per Second: Staves](/dps#staves).

A bonk that can't miss also skips that swing's chance to raise Mace Fighting.

The Shepherd class is built around the shillelagh. See [Character: Classes](/character#classes).

## Manual Training

| Level | Creature | Location |
|:-|:-:|:-:|:-:|
| 1-30 | Sheep | Moonglow Zoo |
| 30-50 | Polar bear | Moonglow Zoo |
| 50-70 | Snow leopard | Moonglow Zoo |
| 70-90 | Bull | Moonglow Zoo |
| 90-100 | Giant Frog | Moonglow Zoo

## Macro Training
Double click the creature you want to train on, then loop:
- `Use Item In Hand`
- `Wait For Target`
- `Last Target`
- `Wait For Target`
- `Last Target`
- `Delay 1000 ms`

It takes 30-60 minutes to grandmaster from scratch.