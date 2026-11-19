---
title: Pet
description: 
published: true
date: 2026-11-19T05:34:19.423Z
tags: 
editor: markdown
dateCreated: 2026-11-16T07:24:49.945Z
---

# Pet
Pets are a type of follower, and [mounts](/mount) are pets too. [Animal tamers](/animal_taming) specialize in capturing and using pets.

Most pets take up `1` follower slot, but strong pets, such as drakes, take `2` slots, and the most powerful pets, such as dragons, take `3` slots. Pets kept in a [stable](/stable) don't use follower slots.

**Pet death is permanent.**

## Pet Training
Pets train their skills by using them, just like players, but twice as quickly. Even if a pet was paralyzed while being tamed and took the skill penalty, its skills can recover and keep training to their maximum. Pets can train each of their [stats](/stats) up to `100`, the same cap as players. A pet that already starts above `100` in a stat, such as a dragon's Strength, can't raise that stat any further. Animal Lore reveals a creature's stats and skills.

## Healing Pets
Pets are healed with bandages using [Veterinary](/veterinary). The range at which a pet can be bandaged grows with Veterinary skill 𐠒:

| Veterinary | Range (tiles) |
|:-|:-:|
| 0 – 24.9 | 1 |
| 25 – 49.9 | 2 |
| 50 – 74.9 | 3 |
| 75 – 99.9 | 4 |
| 100 | 5 |

## Controlling Pets
Animal tamers command pets with phrases like `all follow me` and `dragon kill`. Tamers can control powerful monsters, which makes hunting for loot much easier, provided their pets stay alive and obedient.

Pets can follow their owner into houses. Untamed creatures can't enter houses.

## Loyalty
Every pet has a hidden Loyalty value from `0` to `100`. A newly tamed pet starts at `100`, and Animal Lore shows how happy a pet is.

Once an hour, every pet in the world loses `10` Loyalty. Stabled pets and pets being ridden don't lose Loyalty. A pet that reaches `0` *looks around desperately*, then decides it is better off without a master and goes wild.

An unfed pet at full Loyalty goes wild after about `10` hours.

## Feeding
Drop food on a pet to feed it. Only its favorite food works, which Animal Lore reveals. Each piece of food in the stack has a `50%` chance to add `10` Loyalty, up to the maximum of `100`. If any of it worked, the pet *looks happier*.

Feeding a stack is more reliable than feeding one piece. A stack of `20` almost always fills a pet back to full. There's no limit to how much a pet will eat, so don't drop more than needed, or the rest is wasted.

Food also restores stamina: `15` per piece, minus `50`. A stack of `4` or more is needed to restore any stamina.

## Obeying Commands
Pets don't always obey. Every command has a chance to fail, based on the owner's skills, the pet's difficulty, and its Loyalty. Animal Taming matters four times as much as Animal Lore, and the two combine into a weighted skill:

`Weighted Skill = (4 * Animal Taming + Animal Lore) / 5`

This is compared to the pet's minimum taming skill, the skill needed to tame it:

| Weighted Skill | Chance to Obey (%) |
|:-|:-:|
| Minimum Taming + 4.9 or higher | 99 |
| Equal to Minimum Taming | 70 |
| Below Minimum Taming - 5 | 0 |

Pets that need `29.1` or less to tame, such as horses and ostards, always obey, regardless of their owner's skill or Loyalty. Summoned creatures always obey as well.

For example, with a pet that needs `90` to tame:
- `100` Animal Taming and `100` Animal Lore give a weighted skill of `100`, for a `99%` chance.
- `90` Animal Taming and `100` Animal Lore give a weighted skill of `92`, for an `82%` chance.
- `90` Animal Taming and `50` Animal Lore give a weighted skill of `82`, and the pet will never obey.

Every point of Loyalty below `100` subtracts `1%` from the chance to obey. Pets lose `10` Loyalty an hour, so an unfed pet loses `10%` obedience every hour.

## Stabling Pets
See [Stable](/stable).

## Pack Instinct
Some pets have a Pack Instinct. When an owner controls several pets with the same instinct, they get a damage bonus: `25%` with two pets, `50%` with three, `75%` with four, and `100%` with five. The bonus only affects physical damage, not spells.

- Only pets with the same owner count toward a pack.
- Summoned creatures with the same instinct count.
- Pack members must be attacking the same target and standing within `1` tile of it.

| Pack | Members |
|:-|:-:|
| Bear | Black Bear, Brown Bear, Grizzly Bear, Polar Bear |
| Bull | Bull |
| Canine | Dark Wolf, Dire Wolf, Dog, Grey Wolf, Hell Hound, Timber Wolf, White Wolf |
| Daemon | Fiend, Imp |
| Feline | Cat, Cougar, Hellcat, Panther, Snow Leopard |
| Ostard | Desert Ostard, Forest Ostard, Frenzied Ostard |

## Training on Pets
Players can attack their own pets to train combat skills, and heal them to train Veterinary. 𐠒
- A player's own pets appear green to them, and attacking them is never a criminal act. 𐠒
- Pets don't fight back when attacked.
- Players and their pets can't attack other players' pets.

## Notable Pets
These are some of the most useful creatures to tame.

| Pet | Slots | Skill | Pack Instinct | Notes |
|:-|:-:|:-:|:-:|:-:|
| Horse | 1 | 29.1 | | Mount |
| Forest Ostard | 1 | 29.1 | Ostard | Mount |
| Desert Ostard | 1 | 29.1 | Ostard | Mount |
| Grizzly Bear | 1 | 59.1 | Bear | |
| Bull | 1 | 71.1 | Bull | |
| Frenzied Ostard | 1 | 77.1 | Ostard | Mount |
| Imp | 2 | 83.1 | Daemon | High Magery |
| Drake | 2 | 84.3 | | Fire breath |
| Hell Hound | 1 | 85.5 | Canine | Fire breath |
| Predator Hellcat | 2 | 90 | Feline | Fire breath |
| Silver Steed | 1 | 90 | | Mount, can be Shiny 𐠒 |
| Dragon | 3 | 93.9 | | Fire breath |
| Nightmare | 2 | 100 | | Mount, fire breath, can be Shiny 𐠒 |
| White Wyrm | 3 | 100 | | Highest damage |