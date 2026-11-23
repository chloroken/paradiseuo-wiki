---
title: Pet
description: Training, healing, and commanding pets, plus Pack Instinct and notable pets
published: true
date: 2026-11-20T04:27:23.390Z
tags: 
editor: markdown
dateCreated: 2026-11-16T07:24:49.945Z
---

# Pet
Pets are tamed [followers](/follower), and [mounts](/mount) are pets too. [Animal tamers](/animal_taming) specialize in capturing and using pets. Tamers can control powerful monsters, which makes hunting for loot much easier, provided their pets stay alive and obedient. Loyalty, feeding, and the rules all followers share are on [Follower](/follower).

Most pets take up `1` follower slot, strong pets such as drakes take `2`, and the most powerful pets such as dragons take `3`. See [Follower: Follower Slots](/follower#follower-slots). Pets can be left with an animal trainer while their owner is offline. See [Stable](/stable).

**Pet death is permanent. GMs cannot resurrect pets.**

## Pet Training
Pets train their skills by using them, just like players, but twice as quickly. Even if a pet was paralyzed while being tamed and took the skill penalty, its skills can recover and keep training to their maximum. Pets can train each of their [stats](/stats) up to `100`, the same cap as players. A pet that already starts above `100` in a stat, such as a dragon's Strength, can't raise that stat any further. Animal Lore reveals a creature's stats and skills.

## Healing Pets
Pets are healed with bandages using [Veterinary](/veterinary). The range at which a pet can be bandaged grows with Veterinary skill. See [Veterinary: Range](/veterinary#range). Players can also attack their own pets and bandage them to train Veterinary. See [Follower: Training on Followers](/follower#training-on-followers).

## Pets in Combat
Pets do `25%` less damage to monsters and take `25%` more from them, and a [demiboss](/monsters#demibosses) does double damage to them. Summons share these penalties, but hirelings don't. See [Follower: Followers in Combat](/follower#followers-in-combat).

## Obeying Commands
Pets are commanded with phrases like `all follow me` and `dragon kill`, the same as every follower. See [Follower: Commands](/follower#commands). Unlike hirelings and summons, pets don't always obey. Every command has a chance to fail, based on the owner's skills, the pet's difficulty, and its Loyalty. Animal Taming matters four times as much as Animal Lore, and the two combine into a weighted skill:

`Weighted Skill = (4 * Animal Taming + Animal Lore) / 5`

This is compared to the pet's minimum taming skill, the skill needed to tame it:

| Weighted Skill | Chance to Obey (%) |
|:-|:-:|
| Minimum Taming + 4.9 or higher | 99 |
| Equal to Minimum Taming | 70 |
| Below Minimum Taming - 5 | 0 |

Pets that need `29.1` or less to tame, such as horses and ostards, always obey, regardless of their owner's skill or Loyalty.

For example, with a pet that needs `90` to tame:
- `100` Animal Taming and `100` Animal Lore give a weighted skill of `100`, for a `99%` chance.
- `90` Animal Taming and `100` Animal Lore give a weighted skill of `92`, for an `82%` chance.
- `90` Animal Taming and `50` Animal Lore give a weighted skill of `82`, and the pet will never obey.

Every point of Loyalty below `100` subtracts `1%` from the chance to obey, so an unfed pet obeys less and less. See [Follower: Loyalty](/follower#loyalty).

## Pack Instinct
Some pets have a Pack Instinct. When an owner controls several pets with the same instinct, they get a damage bonus: `25%` with two pets, `50%` with three, `75%` with four, and `100%` with five. The bonus only affects physical damage, not spells.

- Only pets with the same owner count toward a pack.
- Summoned creatures with the same instinct count, but hirelings never do.
- Pack members must be attacking the same target and standing within `1` tile of it.

| Pack | Members |
|:-|:-:|
| Bear | Black bear, brown bear, grizzly bear, polar bear |
| Bull | Bull |
| Canine | Dark wolf, dire wolf, dog, grey wolf, hell hound, timber wolf, white wolf |
| Daemon | Fiend, imp |
| Feline | Cat, cougar, hellcat, panther, snow leopard |
| Ostard | Desert ostard, forest ostard, frenzied ostard |

## Notable Pets
These are some of the most useful creatures to tame.

| Pet | Slots | Skill | Pack Instinct | Notes |
|:-|:-:|:-:|:-:|:-:|
| Horse | 1 | 29.1 | | Mount |
| Forest ostard | 1 | 29.1 | Ostard | Mount |
| Desert ostard | 1 | 29.1 | Ostard | Mount |
| Grizzly bear | 1 | 59.1 | Bear | |
| Bull | 1 | 71.1 | Bull | |
| Frenzied ostard | 1 | 77.1 | Ostard | Mount |
| Imp | 2 | 83.1 | Daemon | High Magery |
| Drake | 2 | 84.3 | | Fire breath |
| Hell hound | 1 | 85.5 | Canine | Fire breath |
| Predator hellcat | 2 | 90 | Feline | Fire breath |
| Silver steed | 1 | 90 | | Mount, can be Shiny |
| Dragon | 3 | 93.9 | | Fire breath |
| Nightmare | 2 | 100 | | Mount, fire breath, can be Shiny |
| White wyrm | 3 | 100 | | Highest damage |