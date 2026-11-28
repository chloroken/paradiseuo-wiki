---
title: Stealing
description: Robbing the pockets of monsters and townsfolk, the lottery, and getting caught
published: true
date: 2026-11-28T13:30:00.000Z
tags: 
editor: markdown
dateCreated: 2026-11-28T13:30:00.000Z
---

# Stealing
Stealing takes items from the pockets of monsters and townsfolk without a fight. Every pocket holds a little loot and a chance at a lottery prize, from a pouch of gems to a castle deed. A thief who isn't caught stays hidden through the whole theft, so [Hiding](/hiding) and [Stealth](/stealth) get them close, [Snooping](/snooping) finds the best item, and [Begging](/begging) or a [vanish](/stealth#vanish) gets them out when things go wrong.

## Stealing from a Creature
Using the skill and targeting a monster or townsperson within `1` tile takes an item from its pocket. Both hands must be free. If a pocket is empty, the thief sees *You find nothing worth stealing.*

Townsfolk are every vendor and every other human NPC who isn't evil. Evil humans, such as brigands and evil mages, are robbed like monsters. Pets, summons, and [hirelings](/hireling) have no pockets.

- The first theft from a creature fills its pocket. A monster's pocket is filled only once, so it slowly empties as it's robbed.
- A townsperson's pocket refills when robbed again after its refresh time, which is set to `2` to `6` hours each time it refills. Anything left from the old pocket is replaced.
- Only pocket items can be stolen. A monster's own gold and loot, and a vendor's shop stock, are never stealable. Townsfolk's gold always counts as part of their pocket.
- Each theft takes a random pocket item, unless [Snooping](/snooping#spotting-prizes) spots a prize.
- Pocket items are deleted when their owner dies, so killing a robbed monster never yields them.
- After each use, the skill can't be used again for `10` seconds.

Stealing from townsfolk requires membership in the [Thieves' Guild](/guilds#thieves-guild). Stealing from players isn't possible, since players [can't attack each other](/rules).

## Getting Away with It
Using Stealing doesn't reveal a hidden thief. Every attempt, successful or not, rolls a chance to be caught: `(10 + (100 - Stealing) / 2)%`, so `10%` at grandmaster and `60%` with no skill. A caught thief is revealed and sees *You have been caught!*

- A monster that catches a thief attacks them.
- A townsperson shouts *Thief!* Inside a guarded town, the thief is taken to [jail](/jail). Outside guarded towns, nothing more happens.
- In the [Karma towns](#karma-towns), getting caught costs Karma instead.

Getting caught never makes a thief a criminal.

## Weight
An item heavier than `10` stones, counting everything inside it, can't be stolen. Heavier items are also harder to take: the chance is `(Stealing - (10 * Weight - 22.5)) / 50`, with weight rounded up to whole stones. At grandmaster, anything up to `7` stones always comes away. From a stack, a thief takes a random amount worth up to `Stealing / 10` stones.

Lottery prizes always count as `1` stone, however heavy they are.

## Pockets
### Townsfolk
What a townsperson carries depends on their work. Each pocket holds gold and has a `50%` chance of one other item.

| Category | Townsfolk | Gold | Other Item |
|:-|:-:|:-:|:-:|
| Wealthy | Bankers, minters, nobles, and jewelers | 80 – 200 | 1 – 3 gems |
| Builder | Real estate brokers and architects | 80 – 200 | 1 – 3 gems |
| Learned | Mages, scribes, alchemists, herbalists, and healers | 40 – 120 | Reagents or a spell scroll |
| Sailor | Shipwrights, fishermen, and mapmakers | 30 – 90 | A gem, or a level 1 treasure map |
| Smith | Blacksmiths, armorers, weaponsmiths, tinkers, and miners | 30 – 90 | 1 – 3 gems |
| Thief | The Thieves' Guild guildmaster | 50 – 150 | A potion |
| Townsfolk | Everyone else | 15 – 60 | A potion |

### Monsters
Monsters never carry gold. Their pockets grow richer with their Fame, and monsters below `1,000` Fame, such as rabbits and rats, have nothing worth taking.

| Fame | Pocket |
|:-|:-:|
| Below 1,000 | Nothing |
| 1,000 – 7,999 | 1 – 2 gems, and a 50% chance of reagents |
| 8,000 – 14,999 | 2 – 4 gems, a potion, and a 50% chance of a spell scroll |
| 15,000+ | 4 – 8 gems, 1 – 2 spell scrolls, and a 10% chance each of a [magic item](/magic_items) and a [wand](/magic_items#wands) |

Spell scrolls in pockets are from circles 1 to 6.

## Lottery
Every pocket rolls once for a lottery prize when it's filled. The prize depends on the owner's category, and falls back to the default when a category has none of its own.

| Prize | Chance | Default | Category Prizes |
|:-|:-:|:-:|:-:|
| Common | 1 in 100 | A pouch of 8 – 15 gems | Learned: a bundle of 5 spell scrolls<br>Sailor: a level 2 treasure map |
| Uncommon | 1 in 1,000 | A bank check for 2,500 gold | Wealthy, learned, and monsters: a strong magic item<br>Sailor: a level 4 treasure map<br>Thief: a skeleton key |
| Rare | 1 in 2,500 | A bank check for 5,000 gold | Wealthy: a bank check for 10,000 gold<br>Learned: a bundle of 3 wands<br>Sailor: a ship deed<br>Builder: a small house deed<br>Monsters: a level 5 treasure map |
| Very rare | 1 in 10,000 | A small house deed | |
| Legendary | 1 in 100,000 | A tower or keep deed | |
| Pipe dream | 1 in 1,000,000 | A castle deed | |

Strong magic items are described on [Magic Items](/magic_items#finding-magic-items). Spell scrolls in bundles are from circles 1 to 6, and ship deeds can be any size.

## Karma Towns
In [Serpent's Hold and Buccaneer's Den](/reputation#karma-towns), stealing from townsfolk needs the same Karma as trading there: `5,000` or more in Serpent's Hold, and `-5,000` or below in Buccaneer's Den. Townsfolk refuse anyone else with the town's usual rebuke.

Neither town sends thieves to jail. Instead, getting caught moves Karma `1,000` toward neutral, even when Karma is [locked](/reputation#karma-lock), and the lock stays as it was. A thief who drops past the town's threshold can't steal or trade there until they rebuild their Karma. These catches never add to a thief's jail record.

Each townsfolk pocket in these towns also rolls for a town prize, separately from the lottery.

| Town | Prize | Chance |
|:-|:-:|:-:|
| Serpent's Hold | A [silver](/magic_weapons#silver) weapon | 1 in 250 |
| Buccaneer's Den | A level 5 [treasure map](/treasure_map) | 1 in 250 |

The silver weapon is any kind of weapon, usually with magic properties, the same as the one the [Lich King](/lich_king#loot) drops.

## Dialogue
| Trigger | Dialogue |
|:-|:-:|
| Starting a theft | *Which item do you want to steal?* |
| An empty pocket | *You find nothing worth stealing.* |
| Snooping spots a prize | *Your keen eye finds something valuable!* |
| Stealing from townsfolk outside the Thieves' Guild | *Only members of the Thieves' Guild may steal from townsfolk.* |
| Getting caught | *You have been caught!* |
| A townsperson catching a thief | *Thief!* |

## Manual Training
A trainer can teach Stealing up to about `30`. From there, monsters are the classroom: every theft trains the skill, and they don't call the guards. At `50`, a thief can join the Thieves' Guild and start working the townsfolk, where the gold is better and the guards are real.

## Macro Training
