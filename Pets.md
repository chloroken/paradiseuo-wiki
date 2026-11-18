---
title: Pets
description: 
published: true
date: 2026-11-18T16:39:22.258Z
tags: 
editor: markdown
dateCreated: 2026-11-16T07:24:49.945Z
---

# Pets
Pets are a type of follower. [Mounts](/Mounts) are pets. [Animal Tamers](/Animal_Taming) specialize in capturing and utilizing pets.

Most pets take up `1` follower slot, but strong pets (e.g., Drakes) take `2` slots and the most powerful pets (e.g., Dragons) take `3` slots. Follower slots are not utilized by pets stored in a [stable](#stables).

**Pet death is permanent.**

## Pet Training
Pets level up skills as they use them just like players do, and they gain skill twice as quickly as players. Even if a pet was paralyzed during taming and it has the skill reduction penalty, its skills can recover and continue training to max. Pets can also train their [stats](/Stats) up to `120`. Using `Animal Lore` reveals a creature's stats and skills.

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

## Loyalty
Every pet has a hidden `Loyalty` value from `0` to `100`. A freshly tamed pet starts at `100`, and Animal Lore shows how happy a pet is.

Once an hour, every pet in the world loses `10` loyalty. Stabled pets and pets being ridden do not lose loyalty. A pet that reaches `0` cries out that it *looks around desperately*, then decides it is better off without a master and goes wild.

An unfed pet at full loyalty goes wild after about `10` hours.

## Feeding
Drop food on a pet to feed it. Only its favorite food works, which Animal Lore reveals. Each piece of food in the stack has a `50%` chance to add `10` loyalty, up to the maximum of `100`. If any of it worked, the pet *looks happier*.

Feeding a stack is more reliable than feeding one piece. A stack of `20` will almost always fill a pet back to full. Note that there is no limit to what a pet will eat, so don't drop more than necessary or it will be wasted.

Food also restores stamina: `15` per piece, minus `50`, which means that stack of `4` or more is required to restore any stamina.

## Obeying Commands
Pets don't always obey. Every command has a chance to fail, based on the owner's skills, the pet's difficulty, and its loyalty. Animal Taming matters four times as much as Animal Lore. The two combine into a weighted skill:

`Weighted Skill = (4 * Animal Taming + Animal Lore) / 5`

This is compared to the pet's `Minimum Taming` skill (the skill needed to tame it):

| Weighted Skill | Chance to Obey |
|:-|:-:|
| `4.9`+ above Minimum Taming | `99%` |
| Equal to Minimum Taming | `70%` |
| Each point above | `+6%` |
| Each point below | `-14%` |
| `3.6` to `5` below | `20%` |
| More than `5` below | `0%` |

For example, with a pet that needs `90` to tame:
- `100` Taming and `100` Lore: weighted `100`, `99%` chance.
- `90` Taming and `100` Lore: weighted `92`, `82%` chance.
- `90` Taming and `50` Lore: weighted `82`, the pet will never obey.

Every point of loyalty below `100` subtracts `1%` from the chance to obey. Since pets lose `10` loyalty an hour, an unfed pet loses `10%` obedience every hour. Thus regular feeding is crucial for pet control.

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

## Training On Pets
Players can attack their own pets to train combat skills, and heal them to train `Veterinary`.
- A player's own pets appear **green** to them, and attacking them is never a criminal act.
- Pets fight back when attacked. Train on a weak pet, since a strong one can kill its owner.
- Players cannot attack other players' pets, and pets cannot attack other players' pets.

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