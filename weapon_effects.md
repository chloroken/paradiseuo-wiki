---
title: Weapon Effects
description: Critical strikes, sapping vigor, Concussion, Crushing, and Paralyzing Blows, the shillelagh, and stun
published: true
date: 2026-11-24T03:30:00.000Z
tags: 
editor: markdown
dateCreated: 2026-11-24T03:30:00.000Z
---

# Weapon Effects
Most weapon types have a weapon effect, which can trigger when a hit lands. Weapon effects are for players only. Monsters, hirelings, and other NPCs never trigger them, even with the same weapons. Some effects also only work against monsters.

Unless noted, each weapon effect is controlled by [Arms Lore](/arms_lore), from nothing at `0` to full strength at `100`. A character without Arms Lore can use any weapon, but never lands its effect. Which weapons have which effect is listed on [Weapons](/weapons#weapon-types).

| Effect | Weapons | Trigger | Works Against |
|:-|:-:|:-:|:-:|
| [Critical strikes](#critical-strikes) | Swords | Each sword's own chance, scaled by Arms Lore | Anything |
| [Sapping vigor](#sapping-vigor) | One-handed maces | Every hit, amount scaled by Arms Lore | Monsters |
| [Concussion Blow](#concussion-blow) | Polearms | Anatomy / 400, no Arms Lore needed | Anything |
| [Crushing Blow](#crushing-blow) | Two-handed maces (war axe, war hammer), staves except the shepherd's crook | Arms Lore / 400 | Monsters |
| [Paralyzing Blow](#paralyzing-blow) | Pitchforks, short spears, spears | Arms Lore / 400 | Anything |
| [Shillelagh](#shillelagh) | Shepherd's crook | First hit after a 9 second cooldown, no Arms Lore needed | Anything |
| [Stun](#stun) | Fists | (Wrestling + Anatomy) / 400, no Arms Lore needed | Anything |

Crushing Blow and Paralyzing Blow each land on `Arms Lore / 400` of hits with the right weapon, which is `25%` at `100` Arms Lore. Three effects don't use Arms Lore: Concussion Blow uses [Anatomy](/anatomy), the shillelagh scales with [Herding](/herding), and stun needs Wrestling and Anatomy. [Crossbow volleys](/archery#crossbow-volley), [poison](/poisoning), and [ambushes](/ambush) aren't weapon effects, so Arms Lore doesn't change them either.

## Critical Strikes
Swords can land a critical strike, which doubles the hit's damage before armor, including a magic weapon's damage bonus. Each sword has its own chance, scaled by Arms Lore, so `50` Arms Lore gives half the chance shown below. The chances are set so every sword does about the same damage over time, and the slowest swords hit in the biggest bursts.

| Sword | Critical Strike Chance (%)<br>at 100 Arms Lore |
|:-|:-:|
| Katana | 12 |
| Broadsword | 10 |
| Scimitar | 15 |
| Cutlass | 17 |
| Longsword | 26 |
| Viking sword | 40 |

Only swords land critical strikes, not axes, polearms, or knives. The attacker sees *You land a critical strike!* in their journal.

## Sapping Vigor
One-handed maces sap a monster's vigor. Each hit saps vigor equal to the damage dealt, scaled by Arms Lore, so `50` Arms Lore saps half as much and a character without Arms Lore saps none. The monster's melee attacks hit as if its Strength were that much lower, down to half its normal Strength. Its health isn't affected. The sap wears off `30` seconds after the last one-handed mace hit from anyone.

The attacker sees *\*saps vigor\** over their head when a sap starts, and everyone nearby sees *\*looks drained of vigor\** when the monster is fully drained. Vigor can only be sapped from monsters.

## Concussion Blow
Polearms can land a Concussion Blow on `Anatomy / 400` of hits, `25%` at `100` Anatomy. It halves the target's Intelligence and lowers its maximum mana for `30` seconds, and doesn't stack. It's aimed at the head, so it uses Anatomy instead of Arms Lore. Two-handed axes don't land it.

Everyone nearby sees *\*looks concussed\** over the target.

## Crushing Blow
Two-handed maces and staves can land a Crushing Blow, which makes the target attack at half speed for `10` seconds. Another Crushing Blow restarts the time instead of stacking. The shepherd's crook is the exception and never lands one.

Crushing Blow only works against monsters. Everyone nearby sees *\*looks dazed\** over the target.

With a two-handed mace, each Crushing Blow has a `Blacksmithing / 100` chance to splash, every time at grandmaster [Blacksmithing](/blacksmithing). Every creature within `1` tile of the target takes the same hit, each reduced by its own armor. Since the splash needs a Crushing Blow first, it needs Arms Lore too. The splash only does damage, with no slow, and gives no skill gains. Staves never splash.

The splash only hits creatures that are fair game: monsters and the creatures they summon. It never hits players, pets, summons, hirelings, or anything innocent, such as townsfolk and animals.

## Paralyzing Blow
Spears, short spears, and pitchforks can land a Paralyzing Blow, which freezes the target in place for `2` seconds.

Everyone nearby sees *\*looks stuck\** over the target.

## Shillelagh
In the hands of a herder, a shepherd's crook becomes a shillelagh. The first crook hit that lands after a `9` second cooldown is a bonk, which multiplies the crook's damage roll by an amount set by Herding. Everyone nearby sees *\*bonk\** over the target. When the cooldown ends, the attacker sees *Your crook hums.* in their journal.

| Herding | Bonk Damage |
|:-|:-:|
| 0 | No bonk |
| 0.1 – 9.9 | 1× |
| 10 – 19.9 | 2× |
| 20 – 29.9 | 3× |
| 30 – 39.9 | 4× |
| 40 – 49.9 | 5× |
| 50 – 59.9 | 6× |
| 60 – 69.9 | 7× |
| 70 – 79.9 | 8× |
| 80 – 89.9 | 9× |
| 90 – 100 | 10× |

- At `100` Herding, a bonk never misses.
- Below `100`, a bonk can miss. A miss shows nothing and doesn't use the bonk, so the next hit that lands bonks instead.
- The multiplier applies to the crook's damage roll, before Tactics, Strength, and Anatomy. A [magic](/magic_weapons) crook's damage bonus is added once and not multiplied, unlike with a critical strike.
- Otherwise a bonk is a normal hit. Armor and shields reduce it, and it's halved against players like all melee between players.
- The cooldown belongs to the player, so switching crooks doesn't reset it.
- The bonk doesn't use Arms Lore.
- Herding adds no damage to the crook's other hits, and the crook never lands a Crushing Blow.

## Stun
Fighting with empty hands allows one move, Stun, which freezes the target in place for `4` seconds. It's attempted automatically when a punch hits, and needs `80` Wrestling and `80` Anatomy, but no Arms Lore. See [Wrestling: Wrestling Moves](/wrestling#wrestling-moves).