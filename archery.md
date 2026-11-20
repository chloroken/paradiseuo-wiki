---
title: Archery
description: 
published: true
date: 2026-11-20T06:46:53.058Z
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
An archer who hides with the [Hiding](/hiding) skill and then attacks with a bow or crossbow ambushes the target, for extra damage.

- A ranged attack that breaks Hiding does `1.5×` damage. This works while mounted.

Moving with [Stealth](/stealth) before the shot makes the ambush stronger.

- Each stealthed step adds `0.1×` damage, capped at a total of `1.0×`.
- Each stealthed step also adds accuracy equal to `10%` of the accuracy missing for a guaranteed hit.
- After `10` stealthed steps, the shot does a total of `2.5×` damage and can't miss. The archer sees *You are in perfect position!* when this is reached, and *You strike with perfect advantage!* on the shot.
- Below `100` Stealth, using Stealth again before the steps run out allows the count to keep going toward `10`.

| Stealthed Steps | Damage | Missing Hit Chance Closed (%) | Hit Chance from 50% (%) |
|:-|:-:|:-:|:-:|
| 0 | 1.5× | 0 | 50 |
| 2 | 1.6× | 20 | 60 |
| 4 | 1.7× | 40 | 70 |
| 6 | 1.8× | 60 | 80 |
| 8 | 1.9× | 80 | 90 |
| 10 | 2.0× | 100 | 100 |

## Restrictions
- Only the Hiding skill counts. Hiding with the [Invisibility](/invisibility) spell or an [invisibility potion](/invisibility_potion) will not trigger ambush.
- Must use Hiding before Stealth, or stealthed steps wont count.
- Once a monster or animal has been damaged by an ambush, it becomes alert for `1` minute. Ambushes on alert targets causes the bonus damage and accuracy being ignored, but don't refresh the alert duration.
- Ambush is capped at `2.0×` damage to players, and players do not become alert when ambushed.

## Dialogue
| Trigger | Dialogue |
|:-|:-:|
| Ambushing from Hiding | *You strike from hiding!* |
| Ambushing from Stealth | *You strike from the shadows!* |
| When maximum stealth step is reached | *You are in perfect position!* |
| Ambushing after taking maximum stealth steps | *You strike with perfect advantage!* |
| Target was too-recently ambushed | *Your target is too alert to ambush!* |

## Valor
Archers with little or no Magery get the same [Valor](/combat#valor) bonuses as any other fighter. Few archers have room for Parrying, so most go without the toughness bonus. Valor and ambushes both apply to the same shot.

## Builds
The stealth archer combines Archery with Hiding and Stealth to open every fight with an ambush. Archery is also a common second weapon skill for bards and fighters, for finishing off fleeing targets. See [Classes](/classes).

## Manual Training
Every shot, hit or miss, has a chance to raise Archery. Attacking one's own [pet](/pet) isn't criminal, so a tamed animal makes a safe training partner, as long as there are arrows or bolts to spare.

## Macro Training