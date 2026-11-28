---
title: Begging
description: Groveling for mercy from monsters, and for gold from townsfolk
published: true
date: 2026-11-28T13:30:00.000Z
tags: 
editor: markdown
dateCreated: 2026-11-28T13:30:00.000Z
---

# Begging
Begging is the art of groveling. A master beggar can plead with a monster that's fighting them until it stops, which gives a thief time to keep working, and anyone can beg townsfolk for a few coins. Using Begging reveals a hidden beggar.

## Begging for Mercy
Begging a monster that's fighting the beggar can [pacify](/peacemaking#pacify) it for `30` seconds. Pacified monsters stop fighting, so a thief can stay put and keep [stealing](/stealing) from the monsters around it.

- It needs `100` Begging. With less, the beggar sees *Only a master beggar could talk their way out of this.*
- The chance to succeed is `(Snooping + Stealing) / 200`, so a grandmaster at both always succeeds.
- Each attempt, successful or not, starts a `2` minute cooldown. This is separate from other skills, so Hiding and Stealth stay ready. Trying too soon shows how long is left, such as *You can beg for mercy again in 1:45.*
- The monster must be fighting the beggar. Otherwise the beggar sees *It isn't threatening you.*, and no cooldown starts.
- Monsters that can't be calmed by [Peacemaking](/peacemaking), including every [demiboss](/demibosses), can't be begged either. This doesn't start the cooldown.
- Stealing from the begged monster ends its pacify, with *It remembers its anger!* Stealing from other monsters doesn't.

Begging monsters never costs Karma.

## Begging for Gold
Begging a human townsperson within `2` tiles asks them for gold. It can't be done while mounted.

- A beggar with negative Karma is often refused with *Thou dost not look trustworthy... no gold for thee today!* The chance is `0.5 - Karma / 8,570`.
- Otherwise, the beggar succeeds `Begging%` of the time. A townsperson gives a tenth of their gold, up to `10` gold, or more for a famous beggar, up to `14` at `10,000` Fame.
- Each success costs up to `40` Karma, but never takes Karma below `-3,000`.

## Dialogue
| Trigger | Dialogue |
|:-|:-:|
| Using the skill | *To whom do you wish to grovel?* |
| A monster is pacified | *Your pitiful groveling stays its hand.* |
| A monster refuses | *Your pleas fall on deaf ears.* |
| A monster that can't be calmed | *Your pleas would mean nothing to such a creature.* |
| A townsperson gives gold | *I feel sorry for thee...* |

## Manual Training
Townsfolk are a patient audience. Begging them for gold trains the skill, so a beggar can work through a town one coin at a time. Expect some Karma to slip away along the way.

## Macro Training
A TazUO Legion script that begs the nearest townsperson at the press of `F1` is on [Scripting](/scripting).
