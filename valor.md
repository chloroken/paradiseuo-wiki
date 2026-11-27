---
title: Valor
description: The warrior's virtue: accuracy, toughness, and regeneration for characters who fight without magic
published: true
date: 2026-11-24T05:55:53.372Z
tags: 
editor: markdown
dateCreated: 2026-11-24T03:38:56.754Z
---

# Valor
Valor is the warrior's virtue. Characters who fight with weapons instead of magic are gripped by it and get three bonuses in combat. The further a character turns toward [magic](/magery), the weaker Valor's hold on them. Valor has nothing to do with the virtue system from later versions of Ultima Online, which *Paradise* doesn't use. Each bonus comes from its own skill and is at its full size with `100` in that skill and `0` Magery. The skill and Magery scales multiply, so a character with `50` in the skill and `50` Magery gets a quarter of the bonus. Only players get these bonuses, not monsters or followers.

## Bonuses
- Accuracy, from [Tactics](/tactics): up to `30` points added to the attacker's weapon skill when rolling to hit, for every kind of weapon, including bows and bare hands. The bonus is `30 * (Tactics / 100) * ((100 - Magery) / 100)` points.
- Toughness, from [Parrying](/parrying): physical damage taken is reduced by up to `20%`, before armor. The reduction is `20% * (Parrying / 100) * ((100 - Magery) / 100)`. It covers weapons and monsters' melee attacks, but not spells, breath, or poison. It doesn't need a shield.
- Regeneration, from [Anatomy](/anatomy): hit points regenerate up to `5` times as fast. The speed is `1 + 4 * (Anatomy / 100) * ((100 - Magery) / 100)` times normal.

| Magery | Accuracy Bonus<br>(points at 100 Tactics) | Damage Taken at<br>100 Parrying (%) | Regeneration Speed<br>at 100 Anatomy |
|:-|:-:|:-:|:-:|
| 0 | 30 | 80 | 5× |
| 25 | 22.5 | 85 | 4× |
| 50 | 15 | 90 | 3× |
| 75 | 7.5 | 95 | 2× |
| 100 | 0 | 100 | 1× |

With `100` Tactics, `100` weapon skill, and no Magery, a fighter hits a defender with `100` skill `60%` of the time instead of `50%`, and hits a monster with `80` Wrestling `69%` of the time instead of `58%`.

The bonuses use base skill, so items and spells that raise a skill don't count. They check the character's skills and Magery at all times, so changing any of them changes the bonuses immediately. These numbers are being tested during alpha and may change.

## Who Gets Valor
Every player gets Valor from their Tactics, Parrying, and Anatomy, whatever they fight with, so archers and wrestlers benefit too. Magery weakens all three bonuses. Fighters with all three skills and no Magery, such as the Warrior [class](/character#classes), get the full bonuses.