---
title: Healing
description: 
published: true
date: 2026-11-19T09:30:04.711Z
tags: 
editor: markdown
dateCreated: 2026-11-19T07:34:36.283Z
---

# Healing
Healing is the skill of treating people with [bandages](/bandage). It heals wounds, cures poison, and can even bring the dead back to life. Its counterpart for creatures is [Veterinary](/veterinary).

To heal, use a bandage on oneself or on someone else. When bandaging someone else, the healer has to stay next to them until the bandage finishes. [Anatomy](/anatomy) raises the amount healed, and is required for curing poison and resurrection.

## Healing Wounds
The chance for a bandage to heal is `(Healing + 10)%`, minus `2%` for each slip. At `90` Healing or higher, bandages never fail unless they slip.

A successful bandage heals a random amount between:
- Minimum: `Anatomy / 5 + Healing / 5 + 3`
- Maximum: `Anatomy / 5 + Healing / 2 + 10`

| Healing and Anatomy | Chance (%) | Healed |
|:-|:-:|:-:|
| 60 | 70 | 27 – 52 |
| 80 | 90 | 35 – 66 |
| 100 | 100 | 43 – 80 |

## Slips
Taking even a single point of damage while applying a bandage causes a slip. Each slip reduces the chance to heal by `2%` and the amount healed by `4`.

## Bandage Speed
Bandaging someone else depends on the healer's Dexterity:

| Dexterity | Delay (s) |
|:-|:-:|
| Below 40 | 5 |
| 40 – 99 | 4 |
| 100+ | 3 |

Bandaging oneself is much slower: `9.4 + 0.6 * (120 - Dexterity) / 10` seconds.

| Dexterity | Self Delay (s) |
|:-|:-:|
| 25 | 15.1 |
| 40 | 14.2 |
| 65 | 12.7 |
| 100 | 10.6 |

## Curing Poison
Bandaging a poisoned target always tries to cure the poison instead of healing, so a poisoned target can't be healed with bandages until the poison is gone. The cure always fails unless the healer's Healing and Anatomy are both `60` or higher. The chance to cure is:

`(Healing - 30) / 50 - (0.1 * Poison Level) - (0.02 * Slips)`

A healer at `100` skill always cures any poison, unless the bandage slips.

| Poison | Level | Chance at 60 (%) | Chance at 80 (%) | Chance at 100 (%) |
|:-|:-:|:-:|:-:|:-:|
| Lesser | 0 | 60 | 100 | 100 |
| Regular | 1 | 50 | 90 | 100 |
| Greater | 2 | 40 | 80 | 100 |
| Deadly | 3 | 30 | 70 | 100 |
| Lethal | 4 | 20 | 60 | 100 |

## Resurrection
With Healing and Anatomy both at `80` or higher, a bandage used on a ghost can bring them back to life. The chance is `(Healing - 68) / 50`, minus `2%` for each slip: `24%` at `80` Healing, and `64%` at `100`. Resurrecting takes `5` seconds longer than a normal bandage, and the ghost chooses whether to accept.

## Manual Training

## Macro Training