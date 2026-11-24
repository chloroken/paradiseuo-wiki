---
title: Animal Lore
description: Examining creatures, commanding pets, healing creatures, and stable slots
published: true
date: 2026-11-24T08:30:00.000Z
tags: 
editor: markdown
dateCreated: 2026-11-24T08:30:00.000Z
---

# Animal Lore
Animal Lore is the knowledge of creatures. It helps [pets](/pet) obey their owner, strengthens bandages on creatures, and adds stable slots. Used as a skill, it examines a creature's stats, skills, and favorite food. Tamers train it alongside [Animal Taming](/animal_taming).

## Examining
Using the skill and targeting a creature within `8` tiles opens a window describing it. Only creatures with an animal, monster, or sea creature body can be examined, so people can't, and neither can dead pets.

Below `100` Animal Lore, only tamed creatures can be examined, whoever owns them. At `100`, wild creatures that can be tamed can be examined too, with a `50%` chance of success. Wild creatures that can't be tamed can never be examined.

The window has three pages:
- Hit points, stamina, and mana, each current and maximum, plus Strength, Dexterity, Intelligence, and armor rating.
- Wrestling, Tactics, Resisting Spells (shown as `Magic Resistance`), Anatomy, Poisoning, Magery, Evaluating Intelligence, and Meditation. A skill below `10` shows as `---`.
- Favorite food, Pack Instinct, and Loyalty.

A pet only eats its favorite food. See [Follower: Feeding](/follower#feeding), [Follower: Loyalty](/follower#loyalty), and [Pet: Pack Instinct](/pet#pack-instinct).

## Commanding Pets
Every command given to a pet has a chance to fail. The owner's Animal Taming and Animal Lore combine into a weighted skill, with Animal Taming counting four times as much:

`Weighted Skill = (4 * Animal Taming + Animal Lore) / 5`

Each point of Animal Lore adds `0.2` to the weighted skill. With `90` Animal Taming and a pet that needs `90` to tame, `100` Animal Lore gives an `82%` chance to obey, but `50` Animal Lore means the pet never obeys. Pets that need `29.1` or less to tame always obey. See [Pet: Obeying Commands](/pet#obeying-commands).

## Healing Creatures
When bandaging a creature, Animal Lore takes the place of [Anatomy](/anatomy). It raises both the minimum and maximum healed by `Animal Lore / 5`, and curing a creature's poison needs `60` Animal Lore. See [Veterinary](/veterinary).

## Stable Slots
Animal Lore counts toward stable slots, alongside Animal Taming and Veterinary. Each point above `95` in Animal Lore adds `1` more slot. See [Stable: Stable Slots](/stable#stable-slots).

## Manual Training

## Macro Training