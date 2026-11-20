---
title: Archery
description: 
published: true
date: 2026-11-20T03:04:50.572Z
tags: 
editor: markdown
dateCreated: 2026-11-19T04:21:12.302Z
---

# Archery
Archery is the skill of fighting with bows and crossbows. Archers attack from a distance, and on *Paradise*, archers who hide and stealth before shooting can ambush their targets for heavy damage.

## Weapons
Archery covers bows, crossbows, and heavy crossbows. Bows fire arrows, and crossbows fire bolts, both made with [Fletching](/fletching). Every shot uses one arrow or bolt from the backpack, whether it hits or misses.

| Weapon | Strength Required | Damage | Speed | Delay at 100 Stamina (s) | Range (tiles) |
|:-|:-:|:-:|:-:|:-:|:-:|
| Bow | 20 | 9 – 41 | 20 | 3.75 | 10 |
| Crossbow | 30 | 8 – 43 | 18 | 4.17 | 8 |
| Heavy crossbow | 40 | 11 – 56 | 10 | 7.5 | 8 |

Damage is before Tactics and the other bonuses. The bow does the most damage over time, while the heavy crossbow hits hardest per shot, which suits an ambush. Delay follows the same formula as every weapon, so it grows as stamina drops. See [Swing Speed](/combat#swing-speed).

An archer has to stand still for `1` second after their last step before they can fire.

All three weapons take both hands, so an archer can't hold a shield. While holding a bow or crossbow, an archer defends with Archery. See [Hit Chance](/combat#hit-chance).

Arrows and bolts that hit a monster or animal have a `40%` chance to land in its backpack, where they can be looted back. Missed shots have a `40%` chance to drop on the ground.

Arrows and bolts can be coated with poison, and are fired before clean ones. Recovered arrows and bolts are always clean. See [Poisoned Weapons](/poisoning#poisoned-weapons).

Tactics, Strength, Anatomy, and weapon quality raise damage the same way as for any other weapon. See [Combat: Damage](/combat#damage).

## Ambush
An archer who hides with the Hiding skill and then attacks with a bow or crossbow ambushes the target, for extra damage. Moving with [Stealth](/stealth) before the shot makes the ambush stronger.

- A shot that breaks Hiding without any stealthed steps does `1.5×` damage. This works while mounted.
- Each stealthed step adds `0.05×` damage, and closes `10%` of the gap between the archer's normal hit chance and a guaranteed hit.
- After `10` stealthed steps, the shot can't miss and does `2.0×` damage. The archer sees *You are in perfect position!* when this is reached, and *You strike with perfect advantage!* on the shot.
- Below `100` Stealth, using Stealth again before the steps run out allows the count to keep going toward `10`.
- Once a monster or animal has been ambushed, hit or miss, nobody can ambush it again for `1` minute. Trying shows *Your target is too alert to ambush!* Players can be ambushed again at any time.
- Only the [Hiding](/hiding) skill counts. Hiding with the [Invisibility](/invisibility) spell or an [invisibility potion](/invisibility_potion) gives no ambush.

| Stealthed Steps | Damage | Missing Hit Chance Closed (%) | Hit Chance from 50% (%) |
|:-|:-:|:-:|:-:|
| 0 | 1.5× | 0 | 50 |
| 2 | 1.6× | 20 | 60 |
| 4 | 1.7× | 40 | 70 |
| 6 | 1.8× | 60 | 80 |
| 8 | 1.9× | 80 | 90 |
| 10 | 2.0× | 100 | 100 |

## Antimage
Archers with little or no Magery get the same [Antimage](/combat#antimage) bonuses as any other fighter: accuracy from Tactics, toughness from Parrying, and regeneration from Anatomy. Few archers have room for Parrying, so most go without the toughness bonus. Antimage and ambushes both apply to the same shot.

## Builds
The stealth archer combines Archery with Hiding and Stealth to open every fight with an ambush. Archery is also a common second weapon skill for bards and fighters, for finishing off fleeing targets. See [Classes](/classes).

## Manual Training
Every shot, hit or miss, has a chance to raise Archery. Attacking one's own [pet](/pet) isn't criminal, so a tamed animal makes a safe training partner, as long as there are arrows or bolts to spare.

## Macro Training