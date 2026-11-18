---
title: Pets
description: 
published: true
date: 2026-11-18T04:28:43.729Z
tags: 
editor: markdown
dateCreated: 2026-11-16T07:24:49.945Z
---

# Pets
Pets are a type of follower. [Mounts](/Mounts) are pets. [Animal Tamers](/Animal_Taming) specialize in capturing and utilizing pets.

Most pets take up `1` follower slot, but strong pets (e.g., Drakes) take `2` slots and the most powerful pets (e.g., Dragons) take `3` slots. Follower slots are not utilized by pets stored in a [stable](#stables).

**Pet death is permanent.** Pets cannot be bonded, so a pet that dies is gone for good.

## Taming Penalty
Taming a creature reduces its [skills](/Skills) (e.g., `Magery`) by `10%`. If it was paralyzed during the tick it was tamed, its skills are reduced by `14%` instead.

## Pet Training
Pets level up skills as they use them just like players do, and they gain skill twice as quickly as players. Even if a pet was paralyzed during taming and it has the skill reduction penalty, its skills can recover and continue training to max. Pets can also train their [stats](/Stats) up to `120`. Using `Animal Lore` reveals a creature's stats and skills.

## Training With Pets
Players can attack their own pets to train combat skills, and heal them to train `Veterinary`.
- A player's own pets appear **green** to them, and attacking them is never a criminal act.
- Pets fight back when attacked. Train on a weak pet, since a strong one can kill its owner.
- Players cannot attack other players' pets, and pets cannot attack other players' pets.

## Healing Pets
Pets are healed with bandages using [Veterinary](/Veterinary). The range at which a pet can be bandaged grows with Veterinary skill:

| Veterinary | Range |
|:-:|:-:|
| 0 – 24.9 | `1` tile |
| 25 – 49.9 | `2` tiles |
| 50 – 74.9 | `3` tiles |
| 75 – 99.9 | `4` tiles |
| 100 | `5` tiles |

## Controlling Pets
Animal Tamers manipulate pets with commands like `all follow me` and `dragon kill`. Because Animal Tamers can control powerful monsters, farming enemies for loot is a breeze. Assuming, of course, that they're able to keep their pets alive (and control them).

Pets can follow their owner into houses. Untamed creatures cannot enter houses.

## Pet Mood
Pet happiness must be managed in order to control pets, lest the Animal Tamer lose control at an inopportune time. Feed them their favorite food to increase happiness. Their favorite food is indicated by using Animal Lore on them.

## Stables
Animal trainers keep pets safe in their stables. Speak these commands near an animal trainer:

| Command | Effect |
|:-|:-|
| `stable` | Stable a pet, for `30` gold (taken from the backpack or bank) |
| `claim` | Choose a pet to claim from the stables |
| `claim <name>` | Quick-claim a pet by name |
| `stablecount` | Show how many stable slots are used and available |

- Stabled pets can be claimed from any animal trainer.
- Pack animals must be unloaded before they can be stabled.
- Dead, summoned, and human creatures cannot be stabled.

Stable slots depend on a character's combined `Animal Taming`, `Animal Lore`, and `Veterinary` skill:

| Combined Skill | Stable Slots |
|:-:|:-:|
| Below 160 | `2` |
| 160 – 199.9 | `3` |
| 200 – 239.9 | `4` |
| 240+ | `5` |

Each point above `95` in Animal Taming, Animal Lore, or Veterinary adds `1` more slot, so a character at `100` in all three has `20` slots.

## Pack Instinct
Some pets have a `Pack Instinct`, and when controlling multiple pets with the same instinct, they get a damage bonus. With two pets, they receive a `25%` bonus, with three, a `50%`, with four, a `75%` bonus, and with five, a `100%` bonus. This damage bonus only affects physical damage, not spells.

- Only pets with the same owner count toward a pack. Summoned creatures with the same instinct count too.
- Pack members must be attacking the same target and standing within `1` tile of it.
- The bonus only applies when pets attack monsters, never players.

| Pack | Members |
|:-:|--|
| **Bear** | Black Bear, Brown Bear, Grizzly Bear, Polar Bear |
| **Bull** | Bulls |
| **Canine** | Dark Wolf, Dire Wolf, Dog, Grey Wolf, Hell Hound, Timber Wolf, White Wolf |
| **Daemon** | Fiend, Imp |
| **Feline** | Cat, Cougar, Hellcat, Panther, Snow Leopard |
| **Ostard** | Desert Ostard, Forest Ostard, Frenzied Ostard |

## Notable Pets
There are many creatures one can tame, but these are notable for having high damage, health, or `Magery`; or being a `mount`, a `pack instinct` animal, or a pet with `shiny` mechanics.

| Pet Type | Slots | Skill | Pack Instinct | Notes |
|:-:|:-:|:-:|:-:|:-|
| **Horse** | 1 | 30.1 |  | Mount |
| **Forest Ostard** | 1 | 34.8 | Ostard | Mount |
| **Desert Ostard** | 1 | 40.0 | Ostard | Mount |
| **Grizzly Bear** | 1 | 59.1 | Bear | |
| **Bull** | 1 | 71.1 | Bull | |
| **Frenzied Ostard** | 1 | 77.1 | Ostard | Mount |
| **Imp** | 2 | 83.1 | Daemon | High Magery |
| **Drake** | 2 | 84.3 | | Fire breath |
| **Hell Hound** | 1 | 85.5 | Canine | Fire breath |
| **Predator Hellcat** | 2 | 90.0 | Feline | Fire breath |
| **Silver Steed** | 1 | 90.0 | | Mount, can be shiny |
| **Dragon** | 3 | 93.9 | | Fire breath |
| **Nightmare** | 2 | 100 | | Mount, fire breath, can be shiny |
| **White Wyrm** | 3 | 100 | | Highest damage |