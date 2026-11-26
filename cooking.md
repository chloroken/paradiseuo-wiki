---
title: Cooking
description: The skill that makes food, its recipes, and effects
published: true
date: 2026-11-26T18:29:05.245Z
tags: 
editor: markdown
dateCreated: 2026-11-26T18:29:05.245Z
---

# Cooking
Cooking is the skill of turning raw ingredients into meals, using a skillet, rolling pin, or other cooking tool. A cook heals when eating, so a chef can stay hungry and save up a burst of healing for a hard fight. Every character has to eat to avoid the penalties of [hunger](#hunger).

## Hunger
Every character has a hidden hunger value from `0` to `20`. It drops by `1` every `5` minutes while the player is online, and each food raises it by its fill value. A character can keep eating as long as hunger is below `20`, even if the food overshoots it. Eating also restores a little stamina.

| Hunger | State | Effect |
|:-|:-|:-|
| 6 – 20 | Fed | None |
| 1 – 5 | Hungry | No hit point regeneration |
| 0 | Starving | Loses `1` hit point per second, down to `1` |

From a full stomach, a character becomes hungry after about `70` minutes and starves after about `100`. A hungry character sees *You are getting hungry. Your wounds won't heal until you eat.* A starving character sees *You are starving! You'll waste away until you eat.*, repeated every `60` seconds. Starvation never kills, and it doesn't interrupt spells, bandages, or meditation.

Young players get the messages but none of the penalties. Ghosts and staff are unaffected.

## Healing from Food
Eating heals a character by `Cooking / 20` hit points, rounded down, for each point of hunger the meal actually fills. A food that overshoots `20` only counts the hunger it filled. There's no cooldown, so a grandmaster cook can heal up to `100` hit points at once by eating from empty.

| Cooking | Healing per Point Filled | Most Healing from Empty |
|:-|:-:|:-:|
| 20 | 1 | 20 |
| 50 | 2 | 40 |
| 100 | 5 | 100 |

Big meals heal the most, since one meal can fill a lot of hunger at once. The tables below list each food's fill value, and the healing columns assume `100` Cooking and enough room in the stomach.

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

| Item | Minimum Skill | Maximum Skill | Materials | Fill | Healing at 100 Cooking |
|:-|:-:|:-:|:-:|:-:|:-:|
| Bread loaf | 0 | 100 | 1 dough | 3 | 15 |
| Cookies | 0 | 100 | 1 cookie mix | 4 | 20 |
| Cake | 0 | 100 | 1 cake mix | 10 | 50 |
| Muffins | 0 | 100 | 1 sweet dough | 4 | 20 |
| Quiche | 0 | 100 | 1 unbaked quiche | 5 | 25 |
| Meat pie | 0 | 100 | 1 unbaked meat pie | 5 | 25 |
| Sausage pizza | 0 | 100 | 1 uncooked sausage pizza | 6 | 30 |
| Cheese pizza | 0 | 100 | 1 uncooked cheese pizza | 6 | 30 |
| Fruit pie | 0 | 100 | 1 unbaked fruit pie | 5 | 25 |
| Peach cobbler | 0 | 100 | 1 unbaked peach cobbler | 5 | 25 |
| Apple pie | 0 | 100 | 1 unbaked apple pie | 5 | 25 |
| Pumpkin pie | 0 | 100 | 1 unbaked pumpkin pie | 5 | 25 |

## Barbecue
Barbecue needs a fire or other heat source nearby. A whole stack of raw food is cooked at once.

| Item | Minimum Skill | Maximum Skill | Materials | Fill | Healing at 100 Cooking |
|:-|:-:|:-:|:-:|:-:|:-:|
| Cooked bird | 0 | 100 | 1 raw bird | 5 | 25 |
| Chicken leg | 0 | 100 | 1 raw chicken leg | 4 | 20 |
| Fish steak | 0 | 100 | 1 raw fish steak | 3 | 15 |
| Fried eggs | 0 | 100 | 1 egg | 4 | 20 |
| Leg of lamb | 0 | 100 | 1 raw leg of lamb | 5 | 25 |
| Cut of ribs | 0 | 100 | 1 raw ribs | 5 | 25 |

## Other Foods
Some foods can't be cooked, but are bought from vendors or found in the world.

| Food | Fill | Healing at 100 Cooking |
|:-|:-:|:-:|
| Roast pig | 20 | 100 |
| Pumpkin | 8 | 40 |
| Ham | 5 | 25 |
| Watermelon | 5 | 25 |
| Fruit basket | 5 | 25 |
| Sausage | 4 | 20 |
| Cheese wheel or wedge | 3 | 15 |
| French bread | 3 | 15 |
| Slab of bacon | 3 | 15 |
| Bowl of vegetables, stew, or soup | 2 | 10 |
| Fruit, vegetables, bacon, or a cheese slice | 1 | 5 |

## Manual Training

## Macro Training