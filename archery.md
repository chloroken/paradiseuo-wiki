---
title: Archery
description: Bows and crossbows, crossbow volleys, ammunition, and the stealth archer's ambush
published: true
date: 2026-11-21T17:43:45.755Z
tags: 
editor: markdown
dateCreated: 2026-11-19T04:21:12.302Z
---

# Archery
Archery is the skill of fighting with bows and crossbows. Archers attack from a distance, and those who hide and stealth before shooting can ambush their targets for heavy damage.

## Valor
Archers with little or no Magery get the same [Valor](/combat#valor) bonuses as any other fighter. Few archers have room for Parrying, so most go without the toughness bonus. Valor and ambushes both apply to the same shot.

## Weapons
Archery covers bows, crossbows, and heavy crossbows. Bows fire arrows, and crossbows fire bolts, both made with [Fletching](/fletching). Every shot uses one arrow or bolt from the backpack, whether it hits or misses, except the crossbow, which fires a volley. Attack speed follows the same formula as every weapon, so it grows as stamina drops. See [Swing Speed](/combat#swing-speed).

| Weapon | Strength Required | Damage | Speed | Delay at 100 Stamina (s) | Range (tiles) |
|:-|:-:|:-:|:-:|:-:|:-:|
| Bow | 20 | 9 – 41 | 20 | 3.75 | 10 |
| Crossbow | 30 | 5 – 14 per bolt | 18 | 4.17 | 8 |
| Heavy crossbow | 40 | 11 – 56 | 10 | 7.5 | 8 |

The bow and crossbow do the most damage over time. The bow reaches farthest, and the crossbow hits most steadily and is best at spreading poison. The heavy crossbow hits hardest per shot, which suits an [ambush](/archery#ambush). Tactics, Strength, Anatomy, and weapon quality raise damage the same way as for any other weapon. See [Combat: Damage](/combat#damage).

### Crossbow Volley
Each crossbow shot fires a volley of up to `3` bolts, as many as the archer carries. Each one uses a bolt from the backpack, and rolls its own hit, damage, and poison. Skill gain, self-poisoning, weapon wear, and a magic crossbow's damage bonus only count once per volley.

### Defense
All three weapons take both hands, so an archer can't hold a shield. While holding a bow or crossbow, an archer defends with Archery. See [Hit Chance](/combat#hit-chance).

## Movement Delay
An archer has to stand still for `1` second after their last step before they can fire. Fletching reduces this movement recovery delay, allowing experienced fletchers to resume attacking more quickly. See [Fletching and Archery](/fletching#fletching-and-archery).

| Fletching | Movement-to-Attack Delay (s) |
|:-|:-:|
| 0 | 1 |
| 25 | 0.875 |
| 50 | 0.75 |
| 75 | 0.625 |
| 100 | 0.5 |

## Ammunition
Arrows and bolts that hit a monster or animal have a `40%` chance to land in its backpack, where they can be looted back. Missed shots have a `40%` chance to drop on the ground, rising with Fletching. See [Ammunition Recovery](/fletching#ammunition-recovery).

Arrows and bolts can be coated with poison, and are fired before clean ones. Recovered arrows and bolts are always clean. See [Poisoned Weapons](/poisoning#poisoned-weapons).

## Ambush
An archer who hides with the [Hiding](/hiding) skill and then attacks with a bow or crossbow ambushes the target, for extra damage.

- A ranged attack that breaks Hiding does `1.5×` damage. This works while mounted.
- A crossbow volley only strengthens its first bolt.

Moving with [Stealth](/stealth) before the shot makes the ambush stronger.

- Each stealthed step adds `0.1×` damage, capped at a total of `1.0×`.
- Each stealthed step also adds accuracy equal to `10%` of the accuracy missing for a guaranteed hit.
- After `10` stealthed steps, the shot does a total of `2.5×` damage and can't miss. The archer sees *You are in perfect position!* when this is reached, and *You strike with perfect advantage!* on the shot.
- Below `100` Stealth, using Stealth again before the steps run out allows the count to keep going toward `10`.

| Stealthed Steps | Damage | Missing Hit Chance Closed (%) | Hit Chance from 50% (%) |
|:-|:-:|:-:|:-:|
| 0 | 1.5× | 0 | 50 |
| 2 | 1.7× | 20 | 60 |
| 4 | 1.9× | 40 | 70 |
| 6 | 2.1× | 60 | 80 |
| 8 | 2.3× | 80 | 90 |
| 10 | 2.5× | 100 | 100 |

### Restrictions
- Only the Hiding skill counts. Hiding with the [Invisibility](/invisibility) spell or an [invisibility potion](/invisibility_potion) won't trigger an ambush.
- Hiding must be used before Stealth, or stealthed steps don't count.
- Once a monster or animal has been damaged by an ambush, it becomes alert for `1` minute. Ambushes on an alert target get no bonus damage or accuracy, and don't refresh the alert duration.
- Ambush is capped at `2.0×` damage to players, and players do not become alert when ambushed.

### Dialogue
| Trigger | Dialogue |
|:-|:-:|
| Ambushing from Hiding | *You strike from hiding!* |
| Ambushing from Stealth | *You strike from the shadows!* |
| Reaching the maximum stealthed steps | *You are in perfect position!* |
| Ambushing after the maximum stealthed steps | *You strike with perfect advantage!* |
| Target was ambushed too recently | *Your target is too alert to ambush!* |

## Manual Training
Every shot, hit or miss, has a chance to raise Archery. Attacking one's own [follower](/follower) isn't criminal, so a tamed animal makes a safe training partner, as long as there are arrows or bolts to spare.

## Macro Training