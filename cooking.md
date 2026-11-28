---
title: Cooking
description: The skill that makes food, its recipes, and effects
published: true
date: 2026-11-28T14:30:00.000Z
tags: 
editor: markdown
dateCreated: 2026-11-26T18:29:05.245Z
---

# Cooking
Cooking is the skill of turning raw ingredients into meals, using a skillet, rolling pin, or other cooking tool. A cook [restores](#eating-as-a-cook) hit points by eating savory food and mana by eating sweets, so a chef can stay hungry and save up a burst for a hard fight. Every character has to eat to avoid the penalties of [hunger](#hunger).

## Hunger
Every character has a hidden hunger value from `0` to `20`. It drops by `1` every `5` minutes while the player is online, and each food raises it by its fill value. A character can keep eating as long as hunger is below `20`, even if the food overshoots it, but must wait `3` seconds between meals. Eating too soon shows *You are still digesting your last meal.* Eating also restores a little stamina.

| Hunger | State | Effect |
|:-|:-|:-|
| 6 – 20 | Fed | None |
| 1 – 5 | Hungry | No hit point regeneration |
| 0 | Starving | Loses `1` hit point per second, down to `1` |

From a full stomach, a character becomes hungry after about `70` minutes and starves after about `100`. A hungry character sees *You are getting hungry. Your wounds won't heal until you eat.* A starving character sees *You are starving! You'll waste away until you eat.*, repeated every `60` seconds. Starvation never kills, and it doesn't interrupt spells, bandages, or meditation.

Young players get the messages but none of the penalties. Ghosts and staff are unaffected.

## Eating as a Cook
Eating restores `Cooking / 10` points, rounded down, for each point of hunger the meal actually fills. Sweets restore mana, and savory food restores hit points. A food that overshoots `20` only counts the hunger it filled. With a meal every `3` seconds, a grandmaster cook can restore up to `200` hit points or mana by eating from empty, or a mix of both.

| Cooking | Restored per Point Filled | Most Restored from Empty |
|:-|:-:|:-:|
| 20 | 2 | 40 |
| 50 | 5 | 100 |
| 100 | 10 | 200 |

Sweets are cookies, cake, muffins, every pie except the meat pie, peach cobbler, and fruit: apples, bananas, coconuts, dates, grapes, lemons, limes, melons, peaches, pears, plums, and fruit baskets. Everything else is savory.

Big meals restore the most per bite. The tables below list each food's fill value, and the last column assumes `100` Cooking and enough room in the stomach.

## Alcohol
Drinking ale, wine, cider, or liquor lowers hunger by `1`, at most once every `10` seconds, so a cook can make room for another meal, even in the middle of a fight. The drinker sees *The drink settles your stomach.* Alcohol never lowers hunger to `5` or below on its own: at hunger `6` or lower, the drink still makes the drinker drunk but shows *Your stomach is already empty.* instead. Hunger can still drop below `6` from the usual drain right after a drink.

Every drink adds drunkenness: `1` for ale, `2` for wine, `3` for cider, and `4` for liquor, up to `60`. Every `5` seconds, a drunk character loses `1` mana and `1` stamina and has a `10%` chance to lose `1` drunkenness, so each point lasts about `50` seconds. Now and then they hiccup with *\*hic\**, and if they aren't mounted, they also turn to face a random direction. When drunkenness runs out, they see *You feel sober.*

## Ingredients

| Item | Minimum Skill | Maximum Skill | Materials |
|:-|:-:|:-:|:-:|
| Sack of flour | 0 | 100 | 2 sheaves of wheat, at a mill |
| Dough | 0 | 100 | 1 open sack of flour, 1 pitcher of water |
| Sweet dough | 0 | 100 | 1 dough, 1 jar of honey |
| Cake mix | 0 | 100 | 1 open sack of flour, 1 sweet dough |
| Cookie mix | 0 | 100 | 1 jar of honey, 1 sweet dough |

## Preparations
Preparations are baked in an oven to make the matching dish.

| Item | Minimum Skill | Maximum Skill | Materials |
|:-|:-:|:-:|:-:|
| Unbaked quiche | 0 | 100 | 1 dough, 1 egg |
| Unbaked meat pie | 0 | 100 | 1 dough, 1 raw ribs |
| Uncooked sausage pizza | 0 | 100 | 1 dough, 1 sausage |
| Uncooked cheese pizza | 0 | 100 | 1 dough, 1 cheese wheel |
| Unbaked fruit pie | 0 | 100 | 1 dough, 1 pear |
| Unbaked peach cobbler | 0 | 100 | 1 dough, 1 peach |
| Unbaked apple pie | 0 | 100 | 1 dough, 1 apple |
| Unbaked pumpkin pie | 0 | 100 | 1 dough, 1 pumpkin |

## Baking
Baking needs an oven nearby.

| Item | Minimum Skill | Maximum Skill | Materials | Fill | Restores at 100 Cooking |
|:-|:-:|:-:|:-:|:-:|:-:|
| Bread loaf | 0 | 100 | 1 dough | 3 | 30 hit points |
| Cookies | 0 | 100 | 1 cookie mix | 4 | 40 mana |
| Cake | 0 | 100 | 1 cake mix | 10 | 100 mana |
| Muffins | 0 | 100 | 1 sweet dough | 4 | 40 mana |
| Quiche | 0 | 100 | 1 unbaked quiche | 5 | 50 hit points |
| Meat pie | 0 | 100 | 1 unbaked meat pie | 5 | 50 hit points |
| Sausage pizza | 0 | 100 | 1 uncooked sausage pizza | 6 | 60 hit points |
| Cheese pizza | 0 | 100 | 1 uncooked cheese pizza | 6 | 60 hit points |
| Fruit pie | 0 | 100 | 1 unbaked fruit pie | 5 | 50 mana |
| Peach cobbler | 0 | 100 | 1 unbaked peach cobbler | 5 | 50 mana |
| Apple pie | 0 | 100 | 1 unbaked apple pie | 5 | 50 mana |
| Pumpkin pie | 0 | 100 | 1 unbaked pumpkin pie | 5 | 50 mana |

## Barbecue
Barbecue needs a fire or other heat source nearby. A whole stack of raw food is cooked at once.

| Item | Minimum Skill | Maximum Skill | Materials | Fill | Restores at 100 Cooking |
|:-|:-:|:-:|:-:|:-:|:-:|
| Cooked bird | 0 | 100 | 1 raw bird | 5 | 50 hit points |
| Chicken leg | 0 | 100 | 1 raw chicken leg | 4 | 40 hit points |
| Fish steak | 0 | 100 | 1 raw fish steak | 3 | 30 hit points |
| Fried eggs | 0 | 100 | 1 egg | 4 | 40 hit points |
| Leg of lamb | 0 | 100 | 1 raw leg of lamb | 5 | 50 hit points |
| Cut of ribs | 0 | 100 | 1 raw ribs | 5 | 50 hit points |

## Other Foods
Some foods can't be cooked, but are bought from vendors or found in the world.

| Food | Fill | Restores at 100 Cooking |
|:-|:-:|:-:|
| Roast pig | 20 | 200 hit points |
| Pumpkin | 8 | 80 hit points |
| Ham | 5 | 50 hit points |
| Watermelon | 5 | 50 mana |
| Fruit basket | 5 | 50 mana |
| Sausage | 4 | 40 hit points |
| Cheese wheel or wedge | 3 | 30 hit points |
| French bread | 3 | 30 hit points |
| Slab of bacon | 3 | 30 hit points |
| Bowl of vegetables, stew, or soup | 2 | 20 hit points |
| Fruit | 1 | 10 mana |
| Vegetables, bacon, or a cheese slice | 1 | 10 hit points |

## Manual Training

## Macro Training
