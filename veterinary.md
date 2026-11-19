---
title: Veterinary
description: 
published: true
date: 2026-11-19T00:16:49.241Z
tags: 
editor: markdown
dateCreated: 2026-11-18T08:02:09.296Z
---

# Veterinary
Veterinary is the skill of healing creatures with [bandages](/bandage). It's the [animal tamer's](/animal_taming) version of [Healing](/healing).

To heal a creature, usually a pet, use a bandage on it and stay in range until it finishes.

## Stable Slots
Veterinary counts toward a character's stable slots, alongside Animal Taming and Animal Lore. See [Stable](/stable#stable-slots).

## Healing
The chance for a bandage to heal is `(Veterinary + 10)%`, minus `2%` for each slip. At `90` Veterinary or higher, bandages never fail unless they slip.

A successful bandage heals a random amount between:
- Minimum: `Animal Lore / 5 + Veterinary / 5 + 3`
- Maximum: `Animal Lore / 5 + Veterinary / 2 + 10`

| Veterinary and Animal Lore | Chance (%) | Healed |
|:-|:-:|:-:|
| 60 | 70 | 27 – 52 |
| 80 | 90 | 35 – 66 |
| 100 | 100 | 43 – 80 |

Pets also heal an extra `1` hit point for every `100` maximum hit points they have.

## Slips
Taking even a single point of damage while applying a bandage causes a slip. Each slip reduces the chance to heal by `2%` and the amount healed by `4`.

## Range
On *Paradise*, veterinarians can bandage from further away. For every `25` points of Veterinary, bandages gain `1` more tile of range when used on creatures.

| Veterinary | Range (tiles) |
|:-|:-:|
| Below 25 | 1 |
| 25 – 49.9 | 2 |
| 50 – 74.9 | 3 |
| 75 – 99.9 | 4 |
| 100+ | 5 |

## Bandage Speed
The time a bandage takes depends on the healer's Dexterity, with an important breakpoint at `40`.

| Dexterity | Delay (s) |
|:-|:-:|
| Below 40 | 5 |
| 40 – 99 | 4 |
| 100+ | 3 |

## Curing Poison
If the veterinarian's Veterinary and Animal Lore are both `60` or higher, bandaging a poisoned target tries to cure it instead of healing it. The chance to cure is:

`(Veterinary - 30) / 50 - (0.1 * Poison Level) - (0.02 * Slips)`

A veterinarian at `100` skill always cures any poison, unless the bandage slips. Each slip lowers the chance by `2%`.

| Poison | Level | Chance at 60 (%) | Chance at 80 (%) | Chance at 100 (%) |
|:-|:-:|:-:|:-:|:-:|
| Lesser | 0 | 60 | 100 | 100 |
| Regular | 1 | 50 | 90 | 100 |
| Greater | 2 | 40 | 80 | 100 |
| Deadly | 3 | 30 | 70 | 100 |
| Lethal | 4 | 20 | 60 | 100 |

## Manual Training
Players can attack their own pets to train weapon skills, then bandage them to train Veterinary. See [Pet](/pet#training-on-pets).

## Macro Training
Get a hearty pet and several thousand bandages, then create a TazUO Assistant macro. Bind it to a key, set its `Journal Trigger` to `*pet*`, and add the following actions:

| Action | Value |
|:-|:-:|
| `Last Target` | |
| `Bandage Target` | |
| `Delay` | `5100` |
| `Say` | `*pet*` |
| `Attack Last` | |

Attack the pet and type `*pet*` to start the macro, and press the keybind to stop it. Adjust the delay to match the Dexterity table in [Bandage Speed](#bandage-speed).
