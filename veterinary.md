---
title: Veterinary
description: 
published: true
date: 2026-11-19T08:00:20.548Z
tags: 
editor: markdown
dateCreated: 2026-11-18T08:02:09.296Z
---

# Veterinary
Veterinary is the skill of healing creatures with [bandages](/bandage). It's the [animal tamer's](/animal_taming) version of Healing.

To heal a creature, usually a pet, use a bandage on it and stay in range until it finishes.

## Stable Slots
Veterinary counts toward a character's stable slots, alongside Animal Taming and Animal Lore. See [Stable Slots](/stable#stable-slots).

## Healing Creatures
Veterinary heals creatures the same way Healing heals people, using Veterinary in place of Healing and Animal Lore in place of Anatomy. The chance to heal, the amount healed, slips, bandage speed, and curing poison all follow the same rules and formulas. See [Healing](/healing).

Creatures also heal an extra `1` hit point for every `100` maximum hit points they have.

## Range
Veterinarians can bandage creatures from a distance. For every `25` points of Veterinary, bandages gain `1` more tile of range when used on creatures.

| Veterinary | Range (tiles) |
|:-|:-:|
| Below 25 | 1 |
| 25 – 49.9 | 2 |
| 50 – 74.9 | 3 |
| 75 – 99.9 | 4 |
| 100+ | 5 |

## Manual Training
Players can attack their own pets to train weapon skills, then bandage them to train Veterinary. See [Training on Pets](/pet#training-on-pets).

## Macro Training
Get a hearty pet and several thousand bandages, then create a TazUO Assistant macro. Bind it to a key, set its `Journal Trigger` to `*pet*`, and add the following actions:

| Action | Value |
|:-|:-:|
| `Last Target` | |
| `Bandage Target` | |
| `Delay` | `5100` |
| `Say` | `*pet*` |
| `Attack Last` | |

Attack the pet and type `*pet*` to start the macro, and press the keybind to stop it. Adjust the delay to match the character's bandage speed. See [Bandage Speed](/healing#bandage-speed).