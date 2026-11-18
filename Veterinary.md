---
title: Veterinary
description: 
published: true
date: 2026-11-18T08:21:10.615Z
tags: 
editor: markdown
dateCreated: 2026-11-18T08:02:09.296Z
---

# Veterinary
`Veterinary` represents the skill of healing creatures with [bandages](/Bandage). It's the [Animal Tamer's](/Animal_Taming) version of [Healing](/Healing).

To heal a creature (usually a pet), use a `bandage` and stay in range until it resolves.

## Healing
The chance for a bandage to heal is `(Veterinary + 10)%`, minus `2%` for each slip. A veterinarian at `90` or more never fails unless the bandage slipped.

The chance for a veterinarian to successfully heal their target is `(Veterinary + 10)%`, minus `slips × 2%`. Once past level `90`, failure only occurs from slippage and range checks.

A successful bandage randomly heals between two ranges:
- **Minimum:** `Animal Lore / 5 + Veterinary / 5 + 3`
- **Maximum:** `Animal Lore / 5 + Veterinary / 2 + 10`

Pets also heal an extra `1` hit point for every `100` maximum hit points they have, so bandages scale slightly with bigger pets. 

| Veterinary & Animal Lore | Chance | Healed |
|:-:|:-:|:-:|
| 60 | `70%` | `27` – `52` |
| 80 | `90%` | `35` – `66` |
| 100 | `100%` | `43` – `80` |

## Slips
Taking even a single point of damage while applying a bandage causes a slip. Slips reduces the chance to heal by `2%` and amount healed by `4`.

## Range
On *Paradise*, veterinarians can bandage from further away. For every `25` points of `Veterinary`, bandages gain another `1` tile of range when used on creatures.

| Skill | Range |
|:-:|:-:|
| < 25 | `1` tile |
| >= 25 | `2` tiles |
| >= 50 | `3` tiles |
| >= 75 | `4` tiles |
| 100 | `5` tiles |

## Bandage Speed
The time a bandage takes depends on the healer's `Dexterity` with a notable breakpoint.

| Dexterity | Delay |
|:-:|:-:|
| < 40 | `5` seconds |
| >= 40 | `4` seconds |
| 100 | `3` seconds |

## Curing Poison
If the veterinarian's `Veterinary` and `Animal Lore` are both `60` or above, when a target is poisoned bandaging it will attempt to cure instead of heal. The chance for a cure to succeed is:

`(Veterinary - 30) / 50 - (0.1 * poisonLevel) - (0.02 * slips)`

Thus, a veterinarian at `100` skill always cures any poison. Each time the bandage slips, the chance drops by `2%`.

| Poison | Level | Chance at 60 Vet | Chance at 80 Vet | Chance at 100 Vet |
|:-|:-:|:-:|:-:|:-:|
| Lesser | `0` | `60%` | `100%` | `100%` |
| Regular | `1` | `50%` | `90%` | `100%` |
| Greater | `2` | `40%` | `80%` | `100%` |
| Deadly | `3` | `30%` | `70%` | `100%` |
| Lethal | `4` | `20%` | `60%` | `100%` |

## Training
Players can attack their own pets to train weapon skills, then bandage them to train `Veterinary`. See [Pets](/Pets) for details. 

## Stable Slots
`Veterinary` levels counts toward a character's stable slots, alongside `Animal Taming` and `Animal Lore`. See [Stables](/Pets#stables).