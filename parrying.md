---
title: Parrying
description: 
published: true
date: 2026-11-20T16:31:06.576Z
tags: 
editor: markdown
dateCreated: 2026-11-20T03:26:26.815Z
---

# Parrying
Parrying is the skill of blocking attacks with a shield. Through [Valor](/combat#valor), it also makes characters who fight without magic tougher, with or without a shield.

An equipped shield also reduces every hit by a flat amount, whether or not it blocks. See [Armor](/armor).

## Blocking
A character holding a shield has a chance to block each weapon attack that hits them. A blocked attack still lands, but the shield stops part of its damage. Body-worn armor then reduces what's left.

Without a shield, attacks are never blocked, whatever the character's Parrying.

A shield's rating grows with Parrying:

`Shield Rating = Parrying * Shield Armor / 200 + 1`

The chance to block is `Parrying - 2 * Shield Rating` percent, and never below `1%`. Against melee attacks, a block stops damage equal to half the shield rating. Against arrows and bolts, it stops the full shield rating. Each block also has a chance to wear down the shield.

Shields with more armor block less often but stop more damage when they do.

## Shields
| Shield | Armor | Block Chance at 50 (%) | Block Chance at 100 (%) | Melee Damage Blocked at 100 | Ranged Damage Blocked at 100 |
|:-|:-:|:-:|:-:|:-:|:-:|
| Buckler | 7 | 44.5 | 91 | 2 | 4 |
| Wooden shield | 8 | 44 | 90 | 2 | 5 |
| Bronze shield | 10 | 43 | 88 | 3 | 6 |
| Metal shield | 11 | 42.5 | 87 | 3 | 6 |
| Wooden kite shield | 12 | 42 | 86 | 3 | 7 |
| Metal kite shield | 16 | 40 | 82 | 4 | 9 |
| Heater shield | 23 | 36.5 | 75 | 6 | 12 |
| Order shield | 30 | 33 | 68 | 8 | 16 |
| Chaos shield | 32 | 32 | 66 | 8 | 17 |

The table is for shields of regular quality at full durability. An exceptional shield has `8` more armor, so it blocks less often and stops more damage per block. A worn shield loses armor as its durability drops, down to half.

Shields are made with [Blacksmithing](/blacksmithing), except the wooden shield, which is made with [Carpentry](/carpentry). Order shields can only be equipped by members of an Order guild, and chaos shields by members of a Chaos guild.

## Valor
Parrying also gives Valor's toughness bonus, which reduces the physical damage a character takes from weapons and monsters' melee attacks. It needs no shield and applies before armor. The bonus grows with Parrying and shrinks as Magery rises. See [Valor](/combat#valor).

## Manual Training
Use a shield to block hits. Maybe a swarm of rats would do the trick..?

## Macro Training